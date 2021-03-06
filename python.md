---
date: 2021-03-05T10:54
---

# Python programming

## PyCon 2020 Talks
* [x] [Anthony Shaw - Why is Python slow](https://www.youtube.com/watch?v=I4nkgJdVZFA)
	- About CPython and PyPy.
	- About AOT and JIT, comparison of speed and language.
	- Takeaways:
      - Speed is about optimisations.
      - Tight loops hurt.
      - Other implementations available.
      - Parallelism improvements are coming.
      - The GC could be improved.
      - $$$ = optimisations.
    
* [x] [Talk: Hannah Stepanek - Let's talk Databases in Python: SQLAlchemy and Alembic](https://www.youtube.com/watch?v=36yw8VC3KU8)
	- ORM (Object Relational Mapper) maps object/model into DB.
    - SQLAlchemy and Alembic.
    - Reflecting database structure and validating model.
    - Constraints, partial indexing and multi column indexes.
    - Functional/expression indexing.

* [x] [Tutorial: Geir Arne Hjelle - Introduction to Decorators: Power Up Your Python Code - YouTube](https://www.youtube.com/watch?v=T8CQwGIsrx4&)
	- Six exercises/decorators:
    	1. Timer
        2. Tracer
        3. Registry
        4. Call counter
        5. Use units
        6. Supertracer


* [x] [Talk: Aly Sivji - If Statements are a Code Smell - YouTube](https://www.youtube.com/watch?v=P0kfKqMHioQ)
	- Replace compound ifs with boolean functions
    - Flatten nested ifs by returning ASAP
    - Replace duplicate ifs by polymorphism
    	- Identify duplicate if statements
        - Identify their functionality
        - Create a base class to model problem
        - Extract conditional block to child class
        - Driver classes improve readability
        - And extendability!
    - SOLID principle:
    	1. Single responsibility
        	- Class should not be jack-of-all-trades.
            - This complicates the possible changes to a class.
        2. Open/closed
        	- Classes may be extended, but not changed.
        3. Liskov substitution
        	- Validation should be equally or less strict as parent class.
            - Implement at least the same functions as the parent.
        4. Interface segregation
        	- Do not bloat interfaces.
        5. Dependency inversion
        	- Consequence of 2 and 3.

* [x] [Talk: Reuven M. Lerner - Function dissection lab -- learn how functions - YouTube](https://www.youtube.com/watch?v=QR9W81P7yTw)
	- `def` does two things: creates function object and assigns it
    - Function objects contain attributes (bytecode and hints)
    - These attributes dictate behaviour e.g. assignment, scoping.


* [x] [Goodbye Print, Hello Debugger! - Nina Zakharenko - Talk - YouTube](https://www.youtube.com/watch?v=5AYIe-3cD-s)
	- `breakpoint()` to interact with code!
    - `from pprint import pprint`
    - `interact` for multi-line code
    - `n` for next, `s` to step in and `c` to continue
    - `l` or `ll` for list or long list (look around)
    - `pp expr`
    - Remove breakpoints in production code.


* [x] [Tutorial: Sebastian Witowski - Modern Python Developer's Toolkit - YouTube](https://www.youtube.com/watch?v=WkUBx3g2QfQ)
	- VS Code, Virtualenv, pyenv, pipenv, pipx, 
    - Cookiecutter, PEP8, Black, Pytest, sphinx, 


* [x] [Talk: Dustin Ingram - Static Typing in Python - YouTube](https://www.youtube.com/watch?v=ST33zDM9vOE)
	- Type hints, type aliases
    - Mypy, pytype, pyre, pyright, pycharm, ...
    	- Mypy vs. pytype
        - Cross-function inference
        - Runtime lenience
    - enforce, typeguard, typo, ducktype, strictconf, ...
    - And eventually vanilla python?
    - Use typing if the code gets confusing.


* [x] [Talk: Russell Keith-Magee - Snakes in a case: Packaging Python apps for distribution - YouTube](https://www.youtube.com/watch?v=WjMDXDHBn1I)
	- Briefcase, in progress packaging of Python apps.


* [x] [Talk: Conor Hoekstra - Beautiful Python Refactoring - YouTube](https://www.youtube.com/watch?v=W-lZttZhsUY)
	- `enumerate` and destructuring.
    - Delete print and enumerate (if index not needed)
    - List comprehension >> Initialise Then Modify
    - Delete ifs that are redundant
    - Use slicing rather than range and iters.
    - Use conditional expression rather than try/except
    - Remove self-explanatory comments
    - Boolean operations or transformations into lambdas
    - Pandas.read_html does ALL the work for us...
    - Thus:
    	1. Know your collections
        1. Know your algorithms
        1. Know your libraries
        
* [x] [Tutorial: Kimberley Fessel - Let's Scrape the Web](https://github.com/kimfetti/Conferences/tree/master/PyCon_2020)
	- Scraping basics, scraping Wikipedia, Selenium.