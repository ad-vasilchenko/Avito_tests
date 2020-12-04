# Avito_tests

# issue 1:
launch:
python -m doctest -v -o NORMALIZE_WHITESPACE task1.py

result:
Trying:
    encode('')
Expecting:
    ''
ok
Trying:
    encode('MAI')
Expecting:
    '-- .- ..'
ok
Trying:
    encode('SOS')
Expecting:
    '... --- ...'
ok
Trying:
    encode('MAI-PYTHON-2019') # doctest: +ELLIPSIS
Expecting:
    '--...'
ok
Trying:
    encode('SOS')
Expecting:
    '... ---
    ...'
ok
1 items had no tests:
    task1
1 items passed all tests:
   5 tests in task1.encode
5 tests in 2 items.
5 passed and 0 failed.


# issue 2:
launch:
python -m pytest task2.py

result:
3 passed in 0.05s

# issue 3:

launch
python task3.py

result:
Ran 4 tests in 0.002s
OK

# issue 4:
launch:
python -m pytest task4.py

result:
4 passed in 0.06s

# issue 5:
launch:
python -m pytest task5.py

