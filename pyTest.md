.vscode/settings.json
-------------------------
{
    "python.linting.pylintEnabled": true,
    "python.linting.enabled": false,
    "python.formatting.provider": "black",
    "python.testing.pytestEnabled": true,
    "python.testing.unittestEnabled": false,
    "python.testing.pytestArgs": [
      "./src/aidd_pvc_python_molecule/tests/unittests", 
    ],
    //"python.pythonPath": "/home/pras/miniconda3/envs/aiddenv/bin/python"
}

pytest commands


=====================================
1) assert 4==x
2) Function Declaration: def test_calculate number
3) Class Declaration: class
4) Validate Error:
	with pytest.raises(ValueError):
		function call to validate
5) pytest Markers:
	a) Skip Test
	   @pytest.mark.skip
	   def test_func_1(): 
	b) Skip test with condition
	   @pytest.mark.skipif(sys.version_info > (3.7)) 
	   def test_func_1():
	c) Call same test with different paramaters
	   @pytest.parameterize("a,b,c", [(1,2,3),("a","b","c")]) 
6) pytest fixtures:
	@pytest.fixture
	def dummy_student():
		return Student("nikhil", 32)
7) pytest fixture function scope
	a) function - default
	b) class
	c) module
	d) package
	e) session
	@pytest.fixture(scope=function)
8) pytest patch (Replace the parameter)
	with patch(
        "aidd_pvc_python_common.event.event_notification.sqs_client",
        sqs_client,
    )
9) pytest mock
	mock_respone = mock.Mock(name="pras", return_value=2)
	myFunc = mock_response

		
