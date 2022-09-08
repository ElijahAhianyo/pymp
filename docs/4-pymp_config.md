# Pymp Config

[_Documentation generated by Documatic_](https://www.documatic.com)

<!---Documatic-section-Codebase Structure-start--->
## Codebase Structure

<!---Documatic-block-system_architecture-start--->
```mermaid
None
```
<!---Documatic-block-system_architecture-end--->

# #
<!---Documatic-section-Codebase Structure-end--->

<!---Documatic-section-pymp.config._get_conf_value-start--->
## [pymp.config._get_conf_value](4-pymp_config.md#pymp.config._get_conf_value)

<!---Documatic-section-_get_conf_value-start--->
<!---Documatic-block-pymp.config._get_conf_value-start--->
<details>
	<summary><code>pymp.config._get_conf_value</code> code snippet</summary>

```python
def _get_conf_value(suffix):
    pymp_name = 'PYMP_' + suffix
    omp_name = 'OMP_' + suffix
    value = None
    for env_name in [pymp_name, omp_name]:
        if env_name in _os.environ:
            _LOGGER.debug('Using %s environment variable: %s.', env_name, _os.environ[env_name])
            value = _os.environ[env_name]
            break
    return value
```
</details>
<!---Documatic-block-pymp.config._get_conf_value-end--->
<!---Documatic-section-_get_conf_value-end--->

# #
<!---Documatic-section-pymp.config._get_conf_value-end--->

[_Documentation generated by Documatic_](https://www.documatic.com)