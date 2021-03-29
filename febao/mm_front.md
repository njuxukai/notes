# mm_front_sub_thread

| server/client | topic                        | init时机   | 模式    |
| ------------- | ---------------------------- | ---------- | ------- |
| client_       | MM_TOPIC_INIT                | init       | pub/sub |
| client_       | MM_TOPIC_MD_PROXY_RAW_MD(s)  | start_work | pub/sub |
| client_       | MM_TOPIC_STRATEGY_SERVICE(s) | start_work | pub/sub |
| client_       | MM_TOPIC_TRADING_RESULT      | start_work | pub/sub |
| client_       | MM_TOPIC_PRICING_DERIVED_MD  | start_work | pub/sub |
| client_       | MM_TOPIC_CALCULATE_RESULT    | start_work | pub/sub |



# mm_front_pub_thread

| server/client | topic                  | init时机 | 模式    |
| ------------- | ---------------------- | -------- | ------- |
| server_       | MM_TOPIC_FRONT_SUMMARY | init     | pub/sub |
|               |                        |          |         |
|               |                        |          |         |

# mm_front_service_thread

| server/client | topic                        | init时机 | 模式    |
| ------------- | ---------------------------- | -------- | ------- |
| server_       | MM_TOPIC_FRONT_SERVICE       | init     | req/rsp |
| client_       | MM_TOPIC_INIT_SERVICE        | init     | req/rsp |
| client_       | MM_TOPIC_TRADING_SERVICE     | init     | req/rsp |
| client_       | MM_TOPIC_CALCULATE_SERVICE   | init     | req/rsp |
| client_       | MM_TOPIC_STRATEGY_SERVICE(s) | init     | req/rsp |

