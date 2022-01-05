# Dynamic Analysis API Interface

Dynamic Analysis Management
(/api-v1/dynamic-analysis)

- /add

To Add a dynamic analysis.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 分析数据 | analysisData | string | yes | |
| 视频ID | videoID | uint | | Logical foreign key |
| 案件ID | caseID | uint | | Logical foreign key  |

---

- /get-total

Get the total number of dynamic analysiss (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get dynamic analysis list (Used for paging).

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
| 主键 | dynamicAnalysisID | uint | Optional | |
| 分析数据 | dynamicData | string | Optional | |
| 视频ID | videoID | uint | Optional | Logical foreign key |
| 案件ID | caseID | uint | Optional | Logical foreign key |

---

- /is-exist

Determine whether the dynamic analysis exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | dynamicAnalysisID | uint | Optional | |
| 分析数据 | dynamicData | string | Optional | |
| 视频ID | videoID | uint | Optional | Logical foreign key |
| 案件ID | caseID | uint | Optional | Logical foreign key |

---

- /delete

Delete the specific dynamic analysis(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | dynamicAnalysisID | uint | Optional | |
| 分析数据 | dynamicData | string | Optional | |
| 视频ID | videoID | uint | Optional | Logical foreign key |
| 案件ID | caseID | uint | Optional | Logical foreign key |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific dynamic analysis.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | dynamicAnalysisID | uint | Optional | |
| 分析数据 | dynamicData | string | Optional | |
| 视频ID | videoID | uint | Optional | Logical foreign key |
| 案件ID | caseID | uint | Optional | Logical foreign key |

---
