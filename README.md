# celery+redis实现定时任务
*celery和kombu版本不一致会抛异常*<br>
KeyError: 'async'<br>
AttributeError: asyn<br>

## 启动异步服务
celery -A tasks worker --loglevel=info<br>
*此时，异步服务已经可用了，但定时任务并没有执行*

## 启动定时任务
celery -A tasks beat
