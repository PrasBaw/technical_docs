# Python Coding Standards
- **__init__.py** should always be blank and should be in every folder.
- **.py file creation** - lowercase and underscore. mol_prop.py
- **Class name** - starting with capital letters, NO underscore ex: MolProp
- **Static variable** - Capitals with underscores ex: _QUERY_LOAD_DYNAMIC_STD_FORMULA_IDS
- **def functio_name** - lowercase and underscores ex: get_dynamic_formula_id
- **def function_return** - ex: def test -> Union[float, None]:
- **def function_parameters** - ex: test(value: float, std_formulas: List)

**Boolean**
- if bCheck instead of (if bCheck == True)
- if not bCheck instead of (if bCheck == False)
- Try to make if and else in one line. ex: x = 1 if y=10 else 0

**Note**
- Try to minimize the number of lines in python code as it affects performance
- Instead of dynamic typing of variable, 
- Every function should have a return type
- every parameter should have a type
- Never use camel case in any naming.
- Avoid unnecessay looping.
- Instead of iter rows use tuples.
  
