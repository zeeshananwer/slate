---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
  - ruby
  - python
  - javascript
  - csharp

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Introduction 

**Version:** v1.0 

# /API/V{VERSION}/APPOINTMENT/TOKEN
## ***POST*** 

### HTTP Request 
`***POST*** /api/v{version}/appointment/token` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/QUICK
## ***POST*** 

### HTTP Request 
`***POST*** /api/v{version}/appointment/quick` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| smsToPatient | query |  | No |  |
| emailToPatient | query |  | No |  |
| smsToSpecialist | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT
## ***POST*** 

### HTTP Request 
`***POST*** /api/v{version}/appointment` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| smsToPatient | query |  | No |  |
| emailToPatient | query |  | No |  |
| smsToSpecialist | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |
| 409 | Conflict |

## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Page | query |  | No |  |
| Size | query |  | No |  |
| From | query |  | No |  |
| To | query |  | No |  |
| Filter | query |  | No |  |
| FacilityId | query |  | No |  |
| ProviderId | query |  | No |  |
| State | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/{APPOINTMENTID}
## ***PUT*** 

### HTTP Request 
`***PUT*** /api/v{version}/appointment/{appointmentId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| appointmentId | path |  | Yes |  |
| smsToPatient | query |  | No |  |
| emailToPatient | query |  | No |  |
| smsToSpecialist | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

## ***DELETE*** 

### HTTP Request 
`***DELETE*** /api/v{version}/appointment/{appointmentId}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| appointmentId | path |  | Yes |  |
| smsToSpecialist | query |  | No |  |
| emailToSpecialist | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/{APPOINTMENTID}/STATE
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment/{appointmentId}/state` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| appointmentId | path |  | Yes |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/TODAY
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment/today` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Page | query |  | No |  |
| Size | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/HISTORY/{YEAR}
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment/history/{year}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Page | query |  | No |  |
| Size | query |  | No |  |
| Year | path |  | Yes |  |
| Month | path |  | Yes |  |
| Day | path |  | Yes |  |
| Filter | query |  | No |  |
| FacilityId | query |  | No |  |
| ProviderId | query |  | No |  |
| State | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/HISTORY/{YEAR}/{MONTH}
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment/history/{year}/{month}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Page | query |  | No |  |
| Size | query |  | No |  |
| Year | path |  | Yes |  |
| Month | path |  | Yes |  |
| Day | path |  | Yes |  |
| Filter | query |  | No |  |
| FacilityId | query |  | No |  |
| ProviderId | query |  | No |  |
| State | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/APPOINTMENT/HISTORY/{YEAR}/{MONTH}/{DAY}
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/appointment/history/{year}/{month}/{day}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Page | query |  | No |  |
| Size | query |  | No |  |
| Year | path |  | Yes |  |
| Month | path |  | Yes |  |
| Day | path |  | Yes |  |
| Filter | query |  | No |  |
| FacilityId | query |  | No |  |
| ProviderId | query |  | No |  |
| State | query |  | No |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/ENDPOINT/TOKEN
## ***POST*** 

### HTTP Request 
`***POST*** /api/v{version}/endpoint/token` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/ENDPOINT/LOCATION/{LOCATION}
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/endpoint/location/{location}` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| location | path |  | Yes |  |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

# /API/V{VERSION}/FACILITY
## ***GET*** 

### HTTP Request 
`***GET*** /api/v{version}/facility` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 401 | Unauthorized |

# /API/V{VERSION}/USER/DEACTIVATE
## ***POST*** 

### HTTP Request 
`***POST*** /api/v{version}/user/deactivate` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| version | path |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | Success |
| 400 | Bad Request |
| 401 | Unauthorized |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
