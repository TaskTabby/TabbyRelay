<img align="right" src="/icon.png" height="256" width="256">

# Tabby Relay
Relay service used for friend connections

> ⚠️ We do **NOT** merge any pull requests. This is only open source for transparency.

## License 
This server is licensed under the MIT license. Please remember not all of our repositories come under the same license

## How to use
This is a hard thing to answer due to this not really being intended for use outside of TaskTabby. As stated earlier, this is only public for transparency. You may do what you please with the code as long as it follows the MIT license. Other than that, feel free to 'borrow' some code if thats what you wish.

A rough explanation is:

- Listen for incoming requests
- Check if request ID is matching to one given by auth server (prevents relay abuse)
- If permitted allow the IP until session expires
- When server recieves RPC event, find the current IP address for the target person (by username) and relay the information. This stops anyone knowing your IP. Also, perform some checks to ensure the information is legit
