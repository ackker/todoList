### todoList
#### 获取任务列表

- 请求地址

  - /todo/task

- 请求方式

  - GET

- 返回值

  ```javascript
  [
      {
          "completed": false,
          "_id": "5c873f3ea3de40165408f956",
          "title": "吃饭"
      },
      {
          "completed": true,
          "_id": "5c873f3ea3de40165408f957",
          "title": "睡觉"
      }
  ]
  ```

#### 添加任务

- 请求地址

  - /todo/addTask

- 请求方式

  - POST

- 参数

  | 参数名 | 必选 | 类型   | 说明     |
  | ------ | ---- | ------ | -------- |
  | title  | 是   | string | 任务名称 |

- 返回值

  ```javascript
  {
      "completed": false,
       "_id": "5c873f3ea3de40165408f956",
       "title": "吃饭"
  }
  ```

#### 删除任务

- 请求地址

  - /todo/deleteTask

- 请求方式

  - GET

- 参数

  | 参数名 | 必选 | 类型   | 说明   |
  | ------ | ---- | ------ | ------ |
  | _id    | 是   | string | 任务id |

#### 清除已完成任务

- 请求地址
  - /todo/clearTask
- 请求方式
  - GET

#### 修改任务

- 请求地址

  - /todo/modifyTask

- 请求方式

  - POST

- 参数

  | 参数名    | 必选 | 类型    | 说明     |
  | --------- | ---- | ------- | -------- |
  | _id       | 是   | string  | 任务id   |
  | title     | 是   | string  | 任务名称 |
  | completed | 是   | boolean | 任务状态 |

#### 更改任务状态

- 请求地址

  - /todo/changeAllTasksComplete

- 请求方式

  - GET

- 参数

  | 参数名 | 必选 | 类型    | 说明     |
  | ------ | ---- | ------- | -------- |
  | status | 是   | boolean | 任务状态 |
