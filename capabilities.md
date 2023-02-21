# Capabilities in mist-cloud

This is an overview of all the capabilities in mist-cloud, along with their default associations to the default roles Admin and Developer. You can create new roles with:

```bash
mist role [role name]
```

A newly created role has no capabilities, but we can add capabilities to it with the command:

```bash
mist capability [capability code] --role [role name]
```

You can add any of the following capabilities:

| Capability code     | Capability description                      | Admin | Developer |
| ------------------- | ------------------------------------------- | ----- | --------- |
| delete_org          | Can delete the organization                 | ✅     |           |
| manage_teams        | Can create teams and assign users to them   | ✅     |           |
| list_teams          | Can see all teams                           | ✅     | ✅         |
| delete_teams        | Can delete teams                            | ✅     |           |
| create_service      | Can create services                         | ✅     | ✅         |
| list_services       | Can see all services and teams              | ✅     | ✅         |
| delete_services     | Can delete services                         | ✅     | ✅         |
| list_capabilities   | Can see which roles have which capabilities | ✅     |           |
| manage_capabilities | Can add capabilities to roles               | ✅     |           |
| assign_roles        | Can assign roles to users                   | ✅     |           |
| list_roles          | Can see all roles                           | ✅     |           |
| delete_roles        | Can delete role                             | ✅     |           |
| list_users          | Can see all users                           | ✅     |           |
| remove_users        | Can remove users from the organization      | ✅     |           |
| manage_apikeys      | Can manage API keys, including events       |       | ✅         |
| manage_secrets      | Can manage secrets                          |       | ✅         |
| read_source_code    | Can read the source code                    | ✅     | ✅         |
| write_source_code   | Can write the source code                   |       | ✅         |
| view_queue          | Can display the contents of the queues      | ✅     |           |
| view_spending       | Can view the unpaid spending                | ✅     |           |