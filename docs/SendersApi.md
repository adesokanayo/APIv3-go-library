# sib_api_v3_sdk.SendersApi

All URIs are relative to *https://api.sendinblue.com/v3*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateSender**](SendersApi.md#CreateSender) | **Post** /senders | Create a new sender
[**DeleteSender**](SendersApi.md#DeleteSender) | **Delete** /senders/{senderId} | Delete a sender
[**GetIps**](SendersApi.md#GetIps) | **Get** /senders/ips | Get all the dedicated IPs for your account
[**GetIpsFromSender**](SendersApi.md#GetIpsFromSender) | **Get** /senders/{senderId}/ips | Get all the dedicated IPs for a sender
[**GetSenders**](SendersApi.md#GetSenders) | **Get** /senders | Get the list of all your senders
[**UpdateSender**](SendersApi.md#UpdateSender) | **Put** /senders/{senderId} | Update a sender

# **CreateSender**
> CreateSenderModel CreateSender(ctx, optional)
Create a new sender

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SendersApiCreateSenderOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SendersApiCreateSenderOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**optional.Interface of CreateSender**](CreateSender.md)| sender&#x27;s name | 

### Return type

[**CreateSenderModel**](createSenderModel.md)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **DeleteSender**
> DeleteSender(ctx, senderId)
Delete a sender

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **senderId** | **int64**| Id of the sender | 

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetIps**
> GetIps GetIps(ctx, )
Get all the dedicated IPs for your account

### Required Parameters
This endpoint does not need any parameter.

### Return type

[**GetIps**](getIps.md)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetIpsFromSender**
> GetIpsFromSender GetIpsFromSender(ctx, senderId)
Get all the dedicated IPs for a sender

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **senderId** | **int64**| Id of the sender | 

### Return type

[**GetIpsFromSender**](getIpsFromSender.md)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetSenders**
> GetSendersList GetSenders(ctx, optional)
Get the list of all your senders

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
 **optional** | ***SendersApiGetSendersOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SendersApiGetSendersOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ip** | **optional.String**| Filter your senders for a specific ip (available for dedicated IP usage only) | 
 **domain** | **optional.String**| Filter your senders for a specific domain | 

### Return type

[**GetSendersList**](getSendersList.md)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateSender**
> UpdateSender(ctx, senderId, optional)
Update a sender

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **senderId** | **int64**| Id of the sender | 
 **optional** | ***SendersApiUpdateSenderOpts** | optional parameters | nil if no parameters

### Optional Parameters
Optional parameters are passed through a pointer to a SendersApiUpdateSenderOpts struct
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | [**optional.Interface of UpdateSender**](UpdateSender.md)| sender&#x27;s name | 

### Return type

 (empty response body)

### Authorization

[api-key](../README.md#api-key), [partner-key](../README.md#partner-key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
