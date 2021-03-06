## sip-tool
A tool written for Python 3.x that traces SIP messages exported to text from Wireshark \*.pcap files. This project is being designed for use within production traces from IP Multimedia Subsystems (IMS), but can be used within any SIP based system. 

### Current Objectives

0. Call-ID to ASCII Art

    - SIP sessions are identified by several static identifers. One of those is a **Call-ID** . This value will appear in every SIP message. So, see if you can write code that identifies the number of unique Call-ID's in our trace.
    - Now see if you can make you program display each unique **Call-ID** to the screen.
    - Each message goes 'from' one IP address, 'to' another IP address. Using the **Call-ID** as a key, nest a list inside of the corresponding value that tracks the IP hops this SIP message makes.
    - Let's try displaying some ASCII art. Parse the unique IP addresses inside of the nested list, and display them at the top of the screen. Next, try making some type of ASCII lines/stars visually indicate the 'hops' these messages are taking. 
    Here is a graphics tool that may be useful: http://www.graphviz.org/content/cluster

0. Parse for Requests or Responses

    - SIP messages are always 1 of 2 types: requests or response
    - Requests are always ALL CAPS English words. The SIP requets are:
      - **ACK**, **BYE**, **CANCEL**, **INFO**, **INVITE**, **MESSAGE**, **NOTIFY**, **OPTIONS**, **PRACK**, **PUBLISH**, **REFER**, **REGISTER**, **SUBSCRIBE**, **UPDATE**
    - Respones are always numbers **100** to **699**.
    - Both SIP requests and responses are indentified in the first line of the SIP message. Look over our trace file, or ask the instructor to explain the characteristics of requests and responses if it is not clear.
    - Write code that identifies the number of requests in the trace
    - Write code that identifies the number of respones in the trace
    - Write code that sorts the types of requests in the trace
    - Write code that sorts the types of responses in the trace

### Contributing Authors

0. Russell Zachary Feeser
    - Alta3 Research - *Project Organizer*
