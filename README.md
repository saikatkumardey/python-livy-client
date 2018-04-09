# Livy Python Client

Livy Client in python for connecting to Livy Server.


# How to install?

    python setup.py install


# How to use?

```python

    from livy.client import HttpClient

    config = {
        'livy.client.http.connection.timeout': '180',#s
        'livy.client.http.job.initial_poll_interval':'0.01',#s
        'livy.client.http.job.max_poll_interval':'1'#s
    }

    client = HttpClient(LIVY_SERVER_URL,load_defaults=True,conf_dict=config)


```