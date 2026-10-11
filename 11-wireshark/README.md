# Network Traffic Analysis with Wireshark

## Objective
Inspect an HTTP POST request in a lab capture and understand what protocol metadata and form fields may be visible to a packet analyst.

## Concepts
Wireshark decodes captured packets into protocol layers. HTTP without TLS does not encrypt request contents, so form fields may be readable in a capture. HTTPS/TLS changes what a passive observer can see, although metadata may remain visible.

## Lab environment and scope
The screenshot shows a display filter for HTTP POST traffic and a packet directed to `/doLogin` using `application/x-www-form-urlencoded`. IP addresses and form values have been redacted in the public copy. Only analyse captures from your own lab or traffic you are authorised to inspect.

## Procedure
1. Start Wireshark and select the interface or open the authorised training capture file.
2. If capturing live traffic, confirm that the interface and network are within scope before starting the capture.
3. Start capture and reproduce only the benign lab action that generates the expected HTTP request, or open the supplied training capture.
4. Stop the capture after the relevant request is observed.
5. Enter the display filter `http.request.method == "POST"` to narrow the packet list to HTTP POST requests.
6. Select the relevant packet and expand the HTTP/Form URL Encoded details to inspect field names and protocol structure.
7. Do not copy passwords or tokens into notes. Record only the protocol, request method, endpoint path, and whether the content is protected by TLS.
8. Save a redacted screenshot or sanitised capture for evidence, then close the capture when finished.

## Observed result
The screenshot shows a POST request to `/doLogin` with content type `application/x-www-form-urlencoded`. The form data was visible in the packet details. The source/destination addresses and form values are obscured in the portfolio copy. This illustrates cleartext HTTP visibility; it does not establish the wider context or authorisation of the original traffic.

## Evidence
![Redacted Wireshark HTTP POST packet](evidence/wireshark-http-post.png)

## Analysis and recommendations
Credentials sent over unencrypted HTTP can be exposed to anyone able to capture the traffic. Use HTTPS/TLS, redirect HTTP to HTTPS, avoid sending secrets over cleartext protocols, and ensure capture files are handled as sensitive data.

## Reference
[Wireshark User's Guide](https://www.wireshark.org/docs/wsug_html_chunked/)
