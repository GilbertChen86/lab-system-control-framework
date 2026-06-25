# 项目名称：CAPA 不符合项管理工具

版本：v2.0

## 项目简介

CAPA 不符合项管理工具是一个基于 PyQt5 的桌面应用程序，专为实验室/质量管理体系设计，用于实现不符合项的全生命周期闭环管理。它覆盖了从发现、记录、分析、处置、实施、验证到关闭的完整流程，并内置了 5WHY、鱼骨图、8D 等深度分析工具。

## 核心功能

- 不符合项全生命周期管理：创建、编辑、删除、状态流转、最终审批
- 必填原因分析：每个不符合项必须填写根本原因和原因分类，确保闭环质量
- 深度分析工具（可选）：集成 5WHY、鱼骨图、8D 分析工具
- 处置要求管理：支持多条处置要求，每条独立跟踪实施、验证和审批
- 举一反三：支持核查记录与跳过机制
- 佐证材料管理：支持上传文件、自动匹配整改要点、自动重命名
- 附件扫描：扫描指定目录，自动匹配并导入附件
- 数据统计：总数、进行中、本月新增、严重不符合项统计

## 技术栈

- Python 3.8+
- PyQt5
- SQLite

## 环境要求

- Windows 7 / 10 / 11
- Python 3.8 或更高版本
- 已安装 pip

## 安装与运行

1. 安装依赖
```bash
pip install -r requirements.txt
```
2. 运行程序
```bash
python main.py
```
3. 打包为 EXE（可选）
```bash
# 安装打包工具
pip install pyinstaller pillow

# 转换图标（如需要）
python -c "from PIL import Image; Image.open('CAPA.png').save('CAPA.ico', format='ICO', sizes=[(256,256)])"

# 打包
pyinstaller --onefile --windowed --icon=CAPA.ico --name="CAPA-tool" --hidden-import=core.db --hidden-import=core.nc_item_manager --hidden-import=core.nc_action_manager --hidden-import=core.nc_extension_manager --hidden-import=core.nc_attachment_manager --hidden-import=core.nc_workflow --hidden-import=core.analysis_5why --hidden-import=core.analysis_fishbone --hidden-import=core.analysis_8d --collect-all PyQt5 main.py
```

打包后的 exe 位于 dist/CAPA-tool.exe。

## 目录结构

```text

capa-tool/
├── main.py                 # 程序入口
├── requirements.txt        # Python 依赖
├── README.md               # 项目说明
├── CAPA.png                # 程序图标
├── data/                   # 数据目录（自动生成）
│   ├── capa.db             # SQLite 数据库
│   └── attachments/        # 附件存储目录
├── core/                   # 核心逻辑模块
│   ├── db.py               # 数据库操作
│   ├── nc_item_manager.py  # 不符合项管理
│   ├── nc_action_manager.py# 处置要求管理
│   ├── nc_extension_manager.py # 举一反三管理
│   ├── nc_attachment_manager.py # 附件管理
│   ├── nc_workflow.py      # 工作流引擎
│   ├── analysis_5why.py    # 5WHY 分析工具
│   ├── analysis_fishbone.py# 鱼骨图分析工具
│   └── analysis_8d.py      # 8D 分析工具
└── ui/
    └── main_window.py      # 主窗口界面

```
## 使用流程
1. 创建不符合项 → 填写基本信息
2. 责任部门确认 → 确认不符合项
3. 原因分析 → 填写根本原因和原因分类（必填）
4. 制定处置要求 → 添加多条处置要求，逐条审批
5. 实施 → 每条处置要求独立添加实施记录
6. 验证 → 每条处置要求独立添加验证记录
7. 处置已批准 → 所有处置要求验证通过后进入下一步
8. 举一反三 → 填写核查记录，或选择跳过
9. 最终审批 → 质量负责人审批，关闭不符合项

## 常见问题

- 根本原因和原因分类是必填项：必须填写后才能流转到“制定中”阶段。
- 实施/验证对话框会自动选中当前行：点击表格中的“实施”或“验证”按钮，会自动对应到该处置要求。
- 附件存放位置：data/attachments/{不符合项编号}/
- 数据库文件：data/capa.db，可用 SQLite 浏览器查看

## 许可证
MIT License

## 作者
Gilbert Chen
