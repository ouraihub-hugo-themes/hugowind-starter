# 🚀 部署设置指南

## 部署到 hugowind.github.io

### 步骤 1：创建 Personal Access Token

1. 访问：https://github.com/settings/tokens/new
2. 填写信息：
   - **Note**: `Deploy to hugowind.github.io`
   - **Expiration**: 选择 `90 days` 或 `No expiration`
   - **Select scopes**: 勾选 `repo` (完整权限)
3. 点击 **"Generate token"**
4. **立即复制 token**（只显示一次！）

### 步骤 2：创建目标仓库

1. 创建组织 `hugowind`（如果还没有）
2. 在该组织下创建仓库 `hugowinds.github.io`
3. 确保仓库是 public 的

### 步骤 3：添加 Secret 到 starter 仓库

1. 访问 starter 仓库的 Settings → Secrets and variables → Actions
2. 点击 **"New repository secret"**
3. 填写：
   - **Name**: `DEPLOY_TOKEN`
   - **Secret**: 粘贴刚才复制的 token
4. 点击 **"Add secret"**

### 步骤 4：触发部署

推送代码到 main 分支，或手动触发 workflow：

1. 访问 Actions 页面
2. 选择 "Deploy to GitHub Pages"
3. 点击 "Run workflow"

### 步骤 5：验证部署

等待 1-2 分钟后访问：https://hugowind.github.io

## Token 权限说明

需要勾选的权限：
- ✅ `repo` - 完整的仓库访问权限

## 故障排除

### 错误：not found deploy key or tokens

**原因**：缺少 `DEPLOY_TOKEN` Secret

**解决**：按照步骤 1-3 添加 token

### 错误：Repository not found

**原因**：目标仓库不存在

**解决**：创建 `hugowind/hugowind.github.io` 仓库

### 错误：Permission denied

**原因**：Token 权限不足

**解决**：确认 token 有 `repo` 权限，且有目标仓库的写入权限
