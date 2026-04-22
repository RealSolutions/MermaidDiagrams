architecture-beta
    group azure(cloud)[Azure]

    service db(database)[MySQL] in azure
    service disk1(disk)[Storage account A] in azure
    service disk2(disk)[Storage account B] in azure
    service server(server)[VM] in azure

    db:L -- R:server
    disk1:T -- B:server
    disk2:T -- B:db
