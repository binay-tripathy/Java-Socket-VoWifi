# Java Screen Sharing Server-Client

## Overview

This Java application demonstrates a basic screen sharing functionality between a server and client. The server captures its screen using the `Robot` class, converts the images to bytes, and sends them to connected clients. Clients receive the images and display them in a graphical user interface.

## Files

- `Server.java`: Server-side code responsible for capturing the screen and transmitting the images to connected clients.
- `Client.java`: Client-side code that connects to the server, receives the screen captures, and displays them in a graphical window.

## How to Run

1. **Compile the Java files:**

    ```bash
    javac Server.java
    javac Client.java
    ```

2. **Run the Server:**

    ```bash
    java Server
    ```

3. **Run the Client:**

    ```bash
    java Client
    ```

4. **Replace the placeholder IP address:**

    In `Client.java`, replace the placeholder IP address (`"10.160.65.83"`) with the actual IP address of the server.

## Dependencies

- **Java SE Development Kit (JDK):**
  
  Ensure you have the necessary JDK installed to compile and run the Java code.

## Configuration and Customization

- **Adjust Capture Frequency:**
  
  Modify the delay in the server's `Thread.sleep()` to control the frequency of screen captures. Smaller values result in more frequent captures.

- **Specify Capture Region:**
  
  The code captures the entire screen. If specific regions need to be captured, adjustments to the `Rectangle` in the `Robot.createScreenCapture()` method may be necessary.

## Security Considerations

- This application is designed for educational purposes and may lack robust security features. It is advisable to implement encryption and authentication mechanisms for a production environment.

## Notes

- This application is a simplified example and may not handle advanced features or security considerations that might be necessary in a production environment.

## License

This code is provided under the [MIT License](LICENSE). Feel free to customize and use it in your projects.
