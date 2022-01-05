# Report API Interface

Report Management
(/api-v1/report)

- /add

To Add a report.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 报告名称 | reportName | string | | |
| 案件ID | caseID | uint | | Logical foreign key |

---

- /get-total

Get the total number of reports (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get report list (Used for paging).

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
| 主键 | reportID | uint | Optional | |
| 报告名称 | reportName | string | Optional | |
| 案件ID | staticAnalysisID | uint | Optional | Logical foreign key |

---

- /is-exist

Determine whether the report exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | reportID | uint | Optional | |
| 报告名称 | reportName | string | Optional | |
| 案件ID | staticAnalysisID | uint | Optional | Logical foreign key |

---

- /delete

Delete the specific report(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | reportID | uint | Optional | |
| 报告名称 | reportName | string | Optional | |
| 案件ID | staticAnalysisID | uint | Optional | Logical foreign key |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific report.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | reportID | uint | Optional | |
| 报告名称 | reportName | string | Optional | |
| 案件ID | staticAnalysisID | uint | Optional | Logical foreign key |

---
