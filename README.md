# 代码提交规范
<type>(<scope>): <subject>

type用于说明commit的类别
feat: 新增功能
fix: bug修复
doc: 文档更新
style: 不影响程序逻辑的代码修改(修改空白字符，格式缩进，补全缺失的分号等，没有改变代码逻辑)
refactor: 重构代码(既没有新增功能，也没有修复bug)
perf: 性能，体验优化
test: 新增测试用例或是更新现有规则
build: 主要的目的是修改项目构建系统(例如gulp,webpack,rollup的配置等)的提交
ci: 主要目的是修改项目继续集成流程(例如Travis,Jenkins,GigLab CI,Circle等)的提交
chore: 不属于以上类型的其他类，比如构建流程，依赖管理
revert: 回滚某个更早之前的提交

# git项目分支管理
永久分支
master
develop
辅助分支(临时分支)
feature-*
功能分支，从develop分出来，最后合并到develop分支上
release
测试环境的稳定分支，从develop分支分出来，在基于该分支分出的bugfix-*分支上面进行bug修复，最终合并到release分支上，待测试完成，该分支合并回develop分支和master分支
bugfix-*
测试阶段进行修复bug使用的分支，修复完成后，再合并回release分支
hotfix-*
线上出现的紧急bug，需要及时修复用此类分支命名,，从master分支切换出来的分支，修复之后合并回master和develop

