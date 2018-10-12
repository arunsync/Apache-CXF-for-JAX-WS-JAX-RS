# Apache-CXF-for-JAX-WS-JAX-RS
===============================

Here is the link to the documentation
http://cxf.apache.org/docs/jax-rs-and-jax-ws.html

Apache CXF is the product of two projects, Celtix and XFire, hence the name CXF.

JAX-WS (It is a Java standard to build web service) is a specification and here are the implementation frameworks
  1. Apache CXF
        a. CXF has top notch Spring support.
        b. CXF also has other things besides just JAX-WS. It has a compliant JAX-RS implementation as well and supports exposing 
          services as both REST and SOAP very well.
        c. CXF has better integration with Spring.
        d. It provides various features like:
            d1. Customization of Logging features
            d2. Inbound and Outbound interceptor
            d3. Application Level security
            d4. Easy Exception handling using custom Fault.
  2. Apache Axis2
        a. This has implementation for both Jax-WS and JAX-RS.
        b. Axis 2 does not seems to have a active releases.
  3. JDK 1.6 
        a. The JAX-WS implementation built into the JDK really is just the basic soap stuff. 
        If you need any of the more complex WS-* things l  ike WS-Security, WS-RM, WS-Policy, etc..., 
        you need to use one of the alternatives like CXF or Metro or Axis2.
        b. lots of stuff not available from the in-jdk JAX-WS impl.
  4. Merto
  
  

Creating SOAP WS using Apache CXF
---------------------------------
SOAP WS can be created in 2 ways.
  1. Java First (Maven Archetype: cxf-jaxws-javafirst)
  2. WSDL First (Maven Archetype: cxf-jaxws-wsdlfirst)
  
  1. Building Java First WS
      a. Open STS
      b. File-> New Maven Project
      c. Filter with "cxf-jaxws-javafirst". Make sure the Group Id is "org.apache.cxf.archetype" and click Next
      d. Provide Group Id and other details for your projects and click finish
      e. Now you can see the project is created and it has 0.
