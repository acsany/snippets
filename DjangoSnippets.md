# Django Snippets

## Create secret key
To get a Django project production ready, you must create a new Django secret key that is not stored in the settings file directly.

```
from django.core.management.utils import get_random_secret_key  
get_random_secret_key()
```
