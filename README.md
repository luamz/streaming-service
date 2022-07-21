# Biting Wire - Streaming Service
Streaming Service Application developed in Python3 by Igor Cruz, Luam Souza and Lucas Fauster.

The app consists of a Service Manager and a Streaming Server. The Service Manager is responsible for coordinating messages and operations, it communicates with the clients and the streaming server through a TCP connection. The Streaming Server is responsible for listing videos and sending them to the clients through a UDP connection.

The application has guest and premium users. Premium users can play videosfor themselves and also create groups for watch parties, they are able to add/remove other users to the group and simultaneously play videos for all of them. Guest users can take part in a group.

Application available in **Engligh** and **Brazilian Portuguese**

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

Most libraries can be downloaded via Pip3 and Tkinter can be installed by running ```sudo apt-get install python3.6-tk```
        
## Running
### As User
To run the application you need to do the following steps:
1. Start the service manager by running
``` python3 service_manager_server/main.py ```

2. In another terminal start the streaming service with:
``` python3 streaming_server/serverUDP.py ```

3. Now you can run as many User Interfaces as you would like with: 
``` python3 interfaces/GUI_login.py ```

### As Admin
To run the admin application you just need to run
``` python3 janelas/GUI_server.py ```
to start the Admin Interface

## Navigation
<table>
    <tr>
        <td> 
          <p align="center" style="padding: 10px">
            <img src="https://user-images.githubusercontent.com/50959073/159812515-4452bc23-a36f-4870-bed1-bab4355e6437.png" width="300">
            <br>
            <em>Login Page</em>
          </p> 
        </td>
        <td> 
          <p align="center">
            <img src="https://user-images.githubusercontent.com/50959073/159812696-6a5037c8-728e-4495-a956-9d11d68cb673.png" width="500">
            <br>
            <em>Home Page</em>
          </p> 
        </td>
    </tr>
     <tr>
        <td> 
          <p align="center" style="padding: 10px">
            <img src="https://user-images.githubusercontent.com/50959073/159812851-0bf401f4-bc0e-4990-a506-9da57714257c.png"  width="500">
            <br>
            <em>Creating Group</em>
          </p> 
        </td>
        <td> 
          <p align="center">
            <img src="https://user-images.githubusercontent.com/50959073/160010497-a18103fc-d714-42bb-b067-ae11b8775a8e.png" width="500">
            <br>
            <em>Adding user to group</em>
          </p> 
        </td>
    </tr>
    
</table>

<p align="center">
    <img src="https://user-images.githubusercontent.com/50959073/160010308-0d7eb96c-7def-46de-a86d-a5928afee369.png" width="800">
    <br>
    <em>Playing a video simultaneously to two users</em>
</p> 

<p align="center">
    <img src="https://user-images.githubusercontent.com/50959073/159813592-68efdcd5-70f9-40e8-866e-552b652e6ff1.png" width="600">
    <br>
    <em>Admin Interface</em>
</p> 
