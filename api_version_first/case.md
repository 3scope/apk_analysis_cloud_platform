# Case API Interface

Case Management
(/api-v1/case)

- /add

To Add a case.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 案件名称 | caseName | string | yes | |
| 静态分析ID | staticAnalysisID | uint | | Logical foreign key |
| 动态分析ID | dynamicAnalysisID | uint | | Logical foreign key  |
| 报告ID | reportID | uint | | |
| 上传者ID | uploaderID | uint | | |
| 上传者名称 | uploaderUsername | string | | |

---

- /get-total

Get the total number of cases (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get case list (Used for paging).

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
| 主键 | caseID | uint | Optional | |
| 案件名称 | caseName | string | Optional | |
| 静态分析ID | staticAnalysisID | uint | Optional | Logical foreign key |
| 动态分析ID | dynamicAnalysisID | uint | Optional | Logical foreign key |
| 报告ID | reportID | uint | Optional | |
| 上传者ID | uploaderID | uint | Optional | |
| 上传者名称 | uploaderUsername | string | Optional | |

---

- /is-exist

Determine whether the case exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | caseID | uint | Optional | |
| 案件名称 | caseName | string | Optional | |
| 静态分析ID | staticAnalysisID | uint | Optional | Logical foreign key |
| 动态分析ID | dynamicAnalysisID | uint | Optional | Logical foreign key  |
| 报告ID | reportID | uint | Optional | |
| 上传者ID | uploaderID | uint | Optional | |
| 上传者名称 | uploaderUsername | string | Optional | |

---

- /delete

Delete the specific case(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | caseID | uint | Optional | |
| 案件名称 | caseName | string | Optional | |
| 静态分析ID | staticAnalysisID | uint | Optional | Logical foreign key |
| 动态分析ID | dynamicAnalysisID | uint | Optional | Logical foreign key  |
| 报告ID | reportID | uint | Optional | |
| 上传者ID | uploaderID | uint | Optional | |
| 上传者名称 | uploaderUsername | string | Optional | |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific case.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 案件名称 | caseName | string | Optional | |
| 静态分析ID | staticAnalysisID | uint | Optional | Logical foreign key |
| 动态分析ID | dynamicAnalysisID | uint | Optional | Logical foreign key  |
| 报告ID | reportID | uint | Optional | |
| 上传者ID | uploaderID | uint | Optional | |
| 上传者名称 | uploaderUsername | string | Optional | |

---
