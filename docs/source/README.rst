``pytest-eosiocdt``: test EOSIO smart contracts using Python

This plugin manages the compilation, deployment and testing of EOSIO smart contracts inside docker containers.

Features
--------

- Detect source deltas and only recompile when needed
- Auto deploy multiple contracts for integration tests
- System contracts already deployed
- Python sugar

Requirements
------------

1. Install Docker & Python 3
2. ``pip install -r requirements.txt``
3. ``pip install .``


Get going fast
--------------

1. In a directory called ``contracts``, create a sub-directory for your smart contract sources.
2. Create a ``manifest.toml`` file in the ``contracts`` directory.

.. code-block:: toml

	[helloworld]
	cdt = '1.7.0'

3. Start Docker
4. Create one or more `pytest tests <https://docs.pytest.org>`_
5. Run ``pytest``