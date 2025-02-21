# 学生数据库系统 🎓

这是一个为freeCodeCamp项目构建的学生数据库管理系统，提供基础的CRUD操作和报表生成功能。

## 主要功能 ✨
- **添加学生记录**：支持多字段信息录入
- **更新学生信息**：通过学号定位并修改记录
- **删除学生**：根据学号移除记录
- **高级搜索**：
  - 按姓名/学号精确查询
  - 按班级/年龄范围筛选
- **数据报表**：
  - 班级学生名单
  - 年龄分布统计
  - 成绩分析报告

## 快速启动 🚀
### 环境要求
- Node.js v14+
- npm 6.x

### 安装步骤
```bash
git clone https://github.com/wangzaiwang-hub/freecodecamp-Build-a-Student-Database.git
cd freecodecamp-Build-a-Student-Database
npm install
```

### 使用示例
```bash
node createStudents.js
> 请选择操作：[1] 添加学生 [2] 查询学生 [3] 生成报表
```

## 项目结构 📁
```
.
├── createStudents.js    # 主程序入口
├── data/                # 数据存储目录
│   └── students.json    # 学生数据库文件
├── test/                # 测试套件
│   └── functionalTests.js  # 功能测试
├── package.json
└── README.md
```

## 测试验证 🧪
运行自动化测试：
```bash
npm test
```
测试覆盖包括：
- 学生记录创建与验证
- 边界值测试（年龄/成绩输入）
- 数据持久化检验

## 开发指南 👨💻
### 数据规范
```json
{
  "id": "FCB202403",       // 学号
  "name": "张三",          // 姓名
  "age": 18,              // 年龄
  "class": "A班",         // 所属班级
  "grades": {             // 成绩
    "math": 90,
    "science": 85
  }
}
```

### 贡献说明
欢迎通过Issue提交建议或PR贡献代码：
1. Fork本仓库
2. 创建特性分支（`git checkout -b feature/新功能`）
3. 提交修改（`git commit -am '添加新功能'`）
4. 推送分支（`git push origin feature/新功能`）
5. 创建Pull Request

## 许可协议 📄
本项目基于 [MIT License](LICENSE) 开放使用

---

🔗 关联freeCodeCamp课程：https://www.freecodecamp.org/learn/back-end-development/
```

如果需要调整细节或补充特定内容，请随时告诉我！
