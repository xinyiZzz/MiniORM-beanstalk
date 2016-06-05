## June 2 2016 9:14 AM

# MiniBeanstalk-BeanstalkORM

* * *


## system function/系统功能

By joining together the SQL statement, lightweight MySQL ORM  
封装put和get，提供简易接口

## Use examples/使用范例

```
from beanstalk_handle import BeanstalkHandle  
beanstalk_handle = BeanstalkHandle(host='127.0.0.1')
beanstalk_handle.put('test', {'save_task': ['aaa', 'bbbb']})
beanstalk_handle.put('test', {'save_task': ['1111', '2222']})
for job_msg, job_body in beanstalk_handle.get('test', infinite_loop=False, num=2):
    print job_msg, job_body
```


## contact/联系方式


609610350@qq.com
