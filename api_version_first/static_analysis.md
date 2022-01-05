# Static Analysis API Interface

Static Analysis Management
(/api-v1/static-analysis)

- /add

To Add a static analysis.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 应用名称 | appName | string | | |
| 应用版本 | appVersion | string | | |
| 安装包大小 | apkSize | uint | | The unit of measurement is **byte** |
| 包名 | packageName | string | | |
| MD5 | md5 | string | | |
| SHA160 | sha160 | string | | |
| SHA256 | sha256 | string | | |
| SDK | sdk | string | | |
| 证书 | certificate | string | | |
| 邮箱 | email | string | | |
| IP地址 | ipAdress | string | | |
| 域名 | domainName | string | | |

Notice: 1MB = 2^10 KB = 2^20 Byte

---

- /get-total

Get the total number of static analysiss (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get static analysis list (Used for paging).

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
| 主键 | staticAnalysisID | uint | Optional | |
| 应用名称 | appName | string | Optional | |
| 应用版本 | appVersion | string | Optional | |
| 安装包大小 | apkSize | uint | Optional | The unit of measurement is **byte** |
| 包名 | packageName | string | Optional | |
| MD5 | md5 | string | Optional | |
| SHA160 | sha160 | string | Optional | |
| SHA256 | sha256 | string | Optional | |
| SDK | sdk | string | Optional | |
| 证书 | certificate | string | Optional | |
| 邮箱 | email | string | Optional | |
| IP地址 | ipAdress | string | Optional | |
| 域名 | domainName | string | Optional | |

---

- /is-exist

Determine whether the static analysis exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | staticAnalysisID | uint | Optional | |
| 应用名称 | appName | string | Optional | |
| 应用版本 | appVersion | string | Optional | |
| 安装包大小 | apkSize | uint | Optional | The unit of measurement is **byte** |
| 包名 | packageName | string | Optional | |
| MD5 | md5 | string | Optional | |
| SHA160 | sha160 | string | Optional | |
| SHA256 | sha256 | string | Optional | |
| SDK | sdk | string | Optional | |
| 证书 | certificate | string | Optional | |
| 邮箱 | email | string | Optional | |
| IP地址 | ipAdress | string | Optional | |
| 域名 | domainName | string | Optional | |

---

- /delete

Delete the specific static analysis(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | staticAnalysisID | uint | Optional | |
| 应用名称 | appName | string | Optional | |
| 应用版本 | appVersion | string | Optional | |
| 安装包大小 | apkSize | uint | Optional | The unit of measurement is **byte** |
| 包名 | packageName | string | Optional | |
| MD5 | md5 | string | Optional | |
| SHA160 | sha160 | string | Optional | |
| SHA256 | sha256 | string | Optional | |
| SDK | sdk | string | Optional | |
| 证书 | certificate | string | Optional | |
| 邮箱 | email | string | Optional | |
| IP地址 | ipAdress | string | Optional | |
| 域名 | domainName | string | Optional | |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific static analysis.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | staticAnalysisID | uint | Optional | |
| 应用名称 | appName | string | Optional | |
| 应用版本 | appVersion | string | Optional | |
| 安装包大小 | apkSize | uint | Optional | The unit of measurement is **byte** |
| 包名 | packageName | string | Optional | |
| MD5 | md5 | string | Optional | |
| SHA160 | sha160 | string | Optional | |
| SHA256 | sha256 | string | Optional | |
| SDK | sdk | string | Optional | |
| 证书 | certificate | string | Optional | |
| 邮箱 | email | string | Optional | |
| IP地址 | ipAdress | string | Optional | |
| 域名 | domainName | string | Optional | |

---
