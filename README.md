# PowerPoint 

This action enables the integration of StackStorm into Microsoft PowerPoint. This pack can be used to convert results of actions from other packs into a slide for convincing senior executives of important things.

## Configuration

The user can provide a corporate PowerPoint template by specifying a path in `powerpoint.yaml`

Copy [powerpoint.yaml.example](./powerpoint.yaml.example) to `/opt/stackstorm/configs/powerpoint.yaml`
and edit as required.

**Note** : When modifying the configuration in `/opt/stackstorm/configs/` please
           remember to tell StackStorm to load these new values by running
           `st2ctl reload --register-configs`

### Make Presentation

Input :

```json
[
  {'layout' : 1 # The layout in the template - 1 based
   'title': 'my first slide'
   'text': 'The content of the slide!'}
]

```
