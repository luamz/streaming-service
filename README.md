# Biting Wire - Streaming Service
Streaming Service Application developed in Python3 by Igor Cruz, Luam Souza and Lucas Fauster.

The app consists of a Service Manager and a Streaming Server. The Service Manager is responsible for coordinating messages and operations, it communicates with the clients and the streaming server through a TCP connection. The Streaming Server is responsible for listing videos and sending them to the clients through a UDP connection.

The application has guest and premium users. Premium users can play videosfor themselves and also create groups for watch parties, they are able to add/remove other users to the group and simultaneously play videos for all of them.

Application available in **Engligh** and **Portuguese**

## Requirements
The application was developed with Python (3.6)

### Libraries
<table>
    <tr>
        <th>Required</th>
        <th>Native to Python3</th>
    </tr>
    <tr>
        <td>
            <ul >
                <li>Opencv-contrib-python<br> (4.5.4.60)</li>
                <li>Imutils (0.5.4)</li>
                <li>Numpy (1.19.5)</li>
                <li>Pillow (8.4.0)</li>
                <li>Tkinter (8.6)</li>
            </ul>
        </td>
        <td>
             <ul>
                <li>Socket</li>
                <li>Threading</li>
                <li>Base64</li>
                <li>Sqlite3</li>
                <li>Pickle</li>
                <li>Logging</li>
            </ul>
        </td>
    </tr> 
</table>

Most libraries can be downloaded via Pip3 and OpenCV can be installed by running ```sudo apt-get install python3.6-tk```
        
## Running
### As User
To run the application you need to do the following steps:
1. Start the service manager by running
``` python3 service_manager_server/main.py ```

2. In another terminal start the streaming service with:
``` python3 streaming_server/serverUDP.py ```

3. Now you can run as many User Interfaces as you would like with: 
``` python3 janelas/GUI_login.py ```

### As Admin
To run the admin application you just need to run
``` python3 janelas/GUI_server.py ```
to start the Admin Interface
