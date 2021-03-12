# mm_trading_sub_thread

| server/client | topic                                | init时机   | 角色    |
| ------------- | ------------------------------------ | ---------- | ------- |
| client        | MM_TOPIC_INIT                        | init       | pub/sub |
| client        | MM_TPOIC_TRADING_RAW_TRADING(s)      | start_work | pub/sub |
| client        | MM_TPOIC_TRADING_RAW_QUERY(s)        | start_work | req/rsp |
| client        | MM_TOPIC_STRATEGY_TRADING_COMMAND(s) | start_work | pub/sub |
| server        | MM_TOPIC_TRADING_SERVICE             | start_work | req/rsp |



# mm_trading_pub_thread



# mm_trading_biz_thread