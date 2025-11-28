# 📝 Homework — 作业共享仓库

![GitHub repo size](https://img.shields.io/github/repo-size/htchen2025/Homework?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/htchen2025/Homework?style=flat-square)

这是我的作业仓库，公开给同学参考与交流。仓库的目的是：集中存放课程作业、参考实现、以及每份作业的说明文档，方便同学学习与讨论。  
在使用本仓库前请务必阅读下面的使用与贡献规则（尤其是学术诚信部分）。

---

## 目录（快速导航）
- [仓库说明](#-仓库说明)
- [快速开始](#-快速开始)
- [目录结构约定](#-目录结构约定)
- [文件与命名规范](#-文件与命名规范)
- [运行/编译示例](#-运行编译示例)
- [提交 / 协作流程（给同学）](#-提交--协作流程给同学)
- [学术诚信与注意事项](#-学术诚信与注意事项)
- [常见问题](#-常见问题)
- [许可证（建议）](#-许可证建议)
- [联系方式](#-联系方式)

---

## 📚 仓库说明
本仓库用于保存课程作业代码与报告，便于同学之间共享参考实现与讨论错误。仓库目标不是替代提交平台（如学校的 LMS），而是作为辅助学习资源与版本记录。

---

## 🚀 快速开始
1. Clone 仓库到本地：
```bash
git clone https://github.com/htchen2025/Homework.git
cd Homework
```
2. 浏览对应课程与作业文件夹，例如：
```text
./課程名/作業_01/
```
3. 阅读作业目录下的 README 或说明文件，查看运行步骤与依赖。

---

## 📂 目录结构约定（示例）
建议每门课程使用一个顶级目录，每次作业一个子目录，个人提交放到以学号或姓名为后缀的文件夹中（避免覆盖）。
```
Homework/
├── course-name-1/
│   ├── hw01/
│   │   ├── README.md        # 作业说明、运行方式
│   │   ├── solution/        # 参考实现（可选）
│   │   └── template/        # 作业模板
│   └── hw02/
├── course-name-2/
└── .gitignore
```

---

## 🔤 文件与命名规范
为保证跨平台（Windows/Linux/macOS）和便于自动化脚本识别，请遵循：
- 文件与文件夹名使用小写，单词间用下划线或连字符：`hw01_solution`, `lab-2`
- 源代码文件：`problem1.cpp`, `solution.m`, `report.tex`
- 文档使用 Markdown 或 PDF：`README.md`, `report.pdf`
- 对于每次提交，写清楚提交信息：`git commit -m "hw01: add solution by zhangsan"`

建议每次作业都包含一个 `README.md`，说明：
- 作业要求摘要
- 运行步骤（命令）
- 依赖（工具、版本）
- 作者/贡献者（如适用）

---

## ▶️ 运行 / 编译 示例
下面给出常见语言的示例命令（视具体作业而定）：

C++ (g++):
```bash
g++ -std=c++17 -O2 -o hw01 problem1.cpp
./hw01
```

MATLAB:
- 在 MATLAB 中打开对应文件夹，运行主脚本：
```matlab
run('main.m')
```

Python:
```bash
python3 main.py
# 或者使用虚拟环境
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python main.py
```

LaTeX (编译报告):
```bash
# 推荐使用 xelatex 或 latexmk
xelatex report.tex
bibtex report
xelatex report.tex
xelatex report.tex
```

---

## 🤝 提交 / 协作流程（给同学）
如果你想为仓库贡献（例如提供示例解法或修正说明），请遵循以下流程：

1. Fork 本仓库（在你的 GitHub 账户下）。
2. 在 fork 仓库中创建新分支：
```bash
git checkout -b feat/yourname-hw01
```
3. 将你的内容放入相应课程/作业目录，更新或新增 `README.md`，并编写清晰的提交信息。
4. 提交并 push：
```bash
git add .
git commit -m "hw01: add solution by YourName (explain assumptions)"
git push origin feat/yourname-hw01
```
5. 在原仓库发起 Pull Request（PR），在 PR 描述里写明：
   - 你提交的是参考实现还是解题思路
   - 是否包含测试用例
   - 你是否允许他人复制/修改（版权说明）
6. 等待合并或维护者反馈。

---

## ⚖️ 学术诚信与注意事项
- 本仓库旨在**辅助学习**，不是替代课程正式提交渠道。请勿将仓库中的内容直接作为课程提交（除非授课教师允许）。
- 遵守学术诚信：抄袭会带来严重后果。若参考他人代码请注明作者与来源。
- 若你是助教或教师，请在合并前确认提交不会泄露考试/作业答案。

---

## ❓ 常见问题
Q: 我可以直接把作业答案上传到这里并公开给所有同学吗？  
A: 技术上可以，但请先确认课程教师或助教是否允许公开答案，避免提前泄题。

Q: 我不想把个人信息（学号/姓名）暴露怎么办？  
A: 可使用学号昵称或仅提交代码而不写明真实姓名。

Q: 如何避免推送大文件（如视频、PDF 大文件）？  
A: 在仓库根目录添加 `.gitignore`，排除大文件或二进制文件；必要时使用 Git LFS（需谨慎）。

示例 .gitignore（建议）:
```
# 二进制 / 临时文件
*.exe
*.o
*.pdf
*.mp4
__pycache__/
.DS_Store
```

---

## 📜 许可证（建议）
代码建议使用 MIT License（宽松、常用）。若作业内容不希望被商用或自由传播，可以考虑更严格的 CC BY-NC（署名-非商业）类许可。若需要我可以帮你生成合适的 LICENSE 文件并说明含义。

---

## ✉️ 联系方式
如果有问题或想贡献，请在 Issues 中提交，或通过 GitHub PR 与我联系。  
欢迎大家互相学习、讨论，但请尊重学术诚信规则。

---

谢谢使用！愿这个仓库成为你学习路上的好帮手。🎓
