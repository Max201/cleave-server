Python Server Cleave
====================

Install
-------

    pip install cleave

How to use
----------
**test.py**
	
    from cleave import server
    
    class MyServer(server.BaseServer):
        def client_handler(self, client):
            client.send('Hello world!')
    
    if __name__ == '__main__':
	    MyServer(host='localhost', port=80, clients=10)

**then in console**

	python test.py