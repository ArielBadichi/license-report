# license report tool
generate license report of a project's dependencies

### install 
```
	npm install -g license-report
```

### usage
simple:
```
	> cd your/project/
	> license-report
```
explicit package.json:
```
	license-report --package=/path/to/package.json
```
customize a field's label:
```
	license-report --report.label.department=division
```
customize a default value (only applicable for some fields):
```
	license-report --department.label=division --department.value=ninjaSquad
```
another registry:
```
	license-report --registry=https://myregistry.com/
```
different outputs:
```
	license-report --output=table
	license-report --output=json
	license-report --output=csv
	license-report --output=csv --delimiter="|"
```
exclude (TBD):
```
	license-report --excluse=async --exclude=rc
```

![screenshot](screenshot.png)

### debug
```
export DEBUG=license-report*
```

see lib/config.js for more details

use [rc](https://github.com/dominictarr/rc) for further customization

![ironSource logo](ironsource.png)