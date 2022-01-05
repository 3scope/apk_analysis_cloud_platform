# Video API Interface

Video Management
(/api-v1/video)

- /add

To Add a video.

Request Method: **POST**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 视频名称 | videoName | string | | |
| 视频时间 | videoTime | string | | |

---

- /get-total

Get the total number of videos (Used for paging).

Request Method: **GET**

Request Parameters:
None

---

- /list

Get video list (Used for paging).

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
| 主键 | videoID | uint | Optional | |
| 视频名称 | videoName | string | Optional | |
| 视频时间 | videoTime | string | Optional | |

---

- /is-exist

Determine whether the video exists.

Request Method: **GET**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | videoID | uint | Optional | |
| 视频名称 | videoName | string | Optional | |
| 视频时间 | videoTime | string | Optional | |

---

- /delete

Delete the specific video(s).

Request Method: **DELETE**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | videoID | uint | Optional | |
| 视频名称 | videoName | string | Optional | |
| 视频时间 | videoTime | string | Optional | |

**Notice**: If all parameters are empty, nothing will be done.

---

- /update

Update the specific video.

Request Method: **PUT**

Request Parameters:
| Significance | Field | Type | Required | Description |
| :-: | :-: | :-: | :-: | :-: |
| 主键 | videoID | uint | Optional | |
| 视频名称 | videoName | string | Optional | |
| 视频时间 | videoTime | string | Optional | |

---
