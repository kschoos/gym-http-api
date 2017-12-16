#Build

In order to use the c++ bindings, several dependencies have to be installed:
- Boost (libboost-all-dev)
- Curl (libcurl4-gnutls-dev)
- Jsoncpp (libjsoncpp-dev)

When compiling your agent with g++, you may have to:
- Add include directories for jsoncpp
- Link to jsoncpp
- Link to curl

An example compilation could look like this:
```g++ random_agent.cpp gym_bindings.cpp -I/usr/include/jsoncpp -ljsoncpp
-lcurl```
