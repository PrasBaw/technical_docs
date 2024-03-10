variable type
typing
Iterators
Generators
Inhertiance
pyDantic

FastAPI = Fast Web Framework.
Uvicorn = ASGI Web Server, Asynchronous server gateway interface.
Pydantic models = Python library to perform data validation.

Important Links:
====================
https://www.youtube.com/watch?v=EdbdEYCBNKk&list=PLHzE1YRqw8tefGsrAOmoz8tW51zFkRJvf&index=2

https://www.youtube.com/watch?v=pegcuKk6eAw&list=PLJKsX2KdvEqEgdXyyJhszqgWELWHdlegD&index=1

https://www.youtube.com/watch?v=at1VVgoK1yg&list=PLubBlcpiVEqzr_9C6ySpELMVq1LAuRl_F

https://www.youtube.com/watch?v=kh3Zo07-8ME =======================(websocket)

============================
pip install fastapi
pip install uvicorn

from fastapi import FastAPI
app=FastAPI()
@app.get("/first")
def getEndpoint():
    return {"name":"prashan"}

============================
uvicorn main:app --reload

Swagger Docs: http://127.0.0.1:8000/docs
ReDoc: http://127.0.0.1:8000/redoc


Steps for testing:
--------------------



