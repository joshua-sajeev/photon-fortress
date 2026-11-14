# Photon Fortress

## Configure IBM Quantum access

The notebook reads your IBM Quantum API token from the `IBM_QUANTUM_TOKEN` environment variable. Do not paste the token into the notebook or commit it to Git.

Set the variable in the environment that launches Jupyter, then start or restart the kernel:

```bash
export IBM_QUANTUM_TOKEN="your-token-here"
jupyter lab
```

In the notebook, `QiskitRuntimeService.save_account` stores the token in the local Qiskit account configuration. Keep that local configuration out of source control. If a token was previously committed or shared, revoke it and create a replacement; deleting it from the current notebook does not remove it from Git history.

Before publishing, clear notebook outputs and review the staged files for credentials or private data.
