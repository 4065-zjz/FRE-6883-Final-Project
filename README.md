# FRE-6883-Final-Project: 
## Evaluate the impact of quarterly earnings report on stock price movement
An earnings surprise occurs when a company's reported quarterly or annual profits are above or below analysts' expectations. The tendency of stock prices to drift (over time) in the direction of earnings surprise post the announcement of earnings is termed as PEAD anomaly. If the element of surprise in the announced earnings is positive in magnitude, the stock prices drift positively and vice versa.

## Environment 
### Configure Microsoft Visual Studio for Using LibCurl (PC users)
- Download the zipped file libcurl-vc16-x86-debug-tatic-ipv6-spi-channel and unzip the file.
- Go to **Properties > Configuration Properties > C/C++ > General** . Add the **libcurl-vc16-x86-debug-tatic-ipv6-spi-channel\include** for **Additional Include Directories**
- Go to **Properties > Configuration Properties > C/C++ > Preprocessor**. Add the
following into **Preprocessor Definitions**:
    _CRT_SECURE_NO_WARNING
    CURL_STATICLIB
- Go to **Properties > Configuration Properties > Linker > General**. Add **libcurl-vc16-x86-debug-tatic-ipv6-spi-channel\lib** for **Additional Library
Directories**.
- Then click **Linker > Input> Additional Dependencies**. Add the following libraries to it:
normaliz.lib
ws2_32.lib
wldap32.lib
crypt32.lib
libcurl_a_debug.lib
advapi32.lib

## Development
### Test-Driven development
We use [google test](https://github.com/google/googletest) to unit test our tasks based on initial designs. Google Test is integrated into the Visual Studio IDE as a default component of the Desktop Development with C++ workload. Feel free to run the unit test cases in **gtest** folder.

## 