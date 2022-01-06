# User API Interface

User Management
(/api-v1/user)

- /add

To Add a user.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 用户名 | username | string | yes | |
| 真实姓名 | realName | string | | |
| 角色 | role | string | yes | There are currently three roles: ordinary, expert, and administrator |
| 邮箱 | email | string | | |
| 简介 | description | string | | |
| 密码 | password | string | | |

---

- /get-total

Get the total number of users (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get user list (Used for paging).

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 页码号 | pageNumber | int | yes | |
| 分页大小 | pageSize | int | yes | |

You can also add some conditions which is in "get-one" api.

---

- /get-one

Get the first match data.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | userID | uint | Optional | |
| 用户名 | username | string | Optional | |
| 真实姓名 | realName | string | Optional | |
| 角色 | role | string | Optional | ordinary, expert, and administrator |
| 邮箱 | email | string | Opthional | |

---

- /is-exist

Determine whether the user exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | userID | uint | Optional | |
| 用户名 | username | string | Optional | |
| 真实姓名 | realName | string | Optional | |
| 角色 | role | string | Optional | ordinary, expert, and administrator |
| 邮箱 | email | string | Opthional | |

---

- /delete

Delete the specific user(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | userID | int | Optional | |
| 用户名 | username | string | Optional | |
| 真实姓名 | realName | string | Optional | |
| 角色 | role | string | Optional | ordinary, expert, and administrator |
| 邮箱 | email | string | Opthional | |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific user.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | userID | int | yes | |
| 用户名 | username | string | Optional | |
| 真实姓名 | realName | string | Optional | |
| 角色 | role | string | Optional | ordinary, expert, and administrator |
| 邮箱 | email | string | Opthional | |
| 简介 | description | string | Opthional | |

---
