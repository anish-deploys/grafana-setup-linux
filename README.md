# Grafana Setup Linux

## What is Grafana ?
<ul>
  <li>Grafana is a free and open source visualization tool mostly used with Prometheus to which monitor metrics.</li>
  <li>Grafana provides various dashboards, charts, graphs, alerts for the particular data source.</li>
  <li>Grafana allows us to query, visualize, explore metrics and set alerts for the data source which can be a system, server, nodes, cluster, etc.</li>
  <li>We can also create our own dynamic dashboard for visualization and monitoring.</li>
  <li>We can save the dashboard and can even share with our team members which is one of the main advantage of Grafana.</li>
</ul>

## Installing Grafana

### We can install Grafana on Linux either by downloading .deb package from Grafana Download page or using apt which is more easier.

### Add the Grafana GPG key in Ubuntu using wget : 

    wget -q -O - https://packages.grafana.com/gpg.key | sudo apt-key add -

### Next, add the Grafana repository to your APT sources :

    sudo add-apt-repository "deb https://packages.grafana.com/oss/deb stable main"

### Refresh your APT cache to update your package lists :

    sudo apt update

### Now proceed with the installation :

    sudo apt install grafana

### Once Grafana is installed, use systemctl to start the Grafana server : 

    sudo systemctl start grafana-server

### Verify that Grafana is running by checking the service’s status :

    sudo systemctl status grafana-server
    sudo systemctl enable grafana-server

### Access Grafana Dashboard & type server IP or name followed by grafana default port 3000.

    http://your_ip:3000

### Here you can see Login page of Grafana now you will have to login with below Grafana default UserName and Password.

    Username – admin
    Password – admin
