# This is a guide how to use virtual environment in jupyter notebook in VScode

**Assume you use uv for dependency management.  
**If you use conda, then you can choose kenrel in VS code.

# 1. Move to your repo.

cd your-repo

# 2. If you have virtual environment, you can skip this step. <br> Generate virtual environment if you did not create in the repo.

uv venv

# 3. Install ipykernel library.

uv add (--dev) ipykernel

# 4. Register your environment in jupyter kernel.

uv run ipython kernel install --user --env VIRTUAL_ENV $(pwd)/.venv --name=(Input env name) --display-name "(Input display name)"

*Please replace "Input env name" and "Input display name" by your preferable names.

# 5. Select your kernel from "Select kernel" on the right upper side of jupyter notebook  
