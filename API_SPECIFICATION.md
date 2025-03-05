# 3Xbang API规范

## 认证API

### 登录
- **URL**: `/api/auth/login`
- **方法**: `POST`
- **参数**:
  ```json
  {
    "email": "用户邮箱",
    "password": "密码"
  }
  ```
- **响应**:
  ```json
  {
    "success": true,
    "token": "JWT令牌",
    "user": {
      "id": "用户ID",
      "name": "用户名",
      "email": "用户邮箱",
      "role": "角色"
    }
  }
  ```

## 项目API

### 获取项目列表
- **URL**: `/api/projects`
- **方法**: `GET`
- **响应**:
  ```json
  {
    "success": true,
    "data": [
      {
        "id": "项目ID",
        "name": "项目名称",
        "status": "项目状态",
        "client": "客户信息",
        "startDate": "开始日期",
        "endDate": "结束日期"
      }
    ]
  }
  ```
