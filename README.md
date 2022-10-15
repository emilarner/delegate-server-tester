# delegate-server-tester

Tests if a Delegate server implementation complies with the Delegate protocol standard.

Because the Delegate Protocol and the corresponding Python server implementation are not finished, this tool is not finished either... but it works for most Phase 1 thing (see the Delegate Server implementation repository to see what each phase contains). This tool will test various features and see if they return the expected result... It should look something like this. You need to pass in the WebSocket address of the server you want to test in for the first argument, and the server you are testing needs to have a clean slate (its database is empty; you can clear it with reset-db.py in the server implementation repo).

    Testing JSON sanity checking...
    'JSON sanity checking'... PASSED ✓ 
    
    Testing user registration...
    'user registration'... PASSED ✓ 
    
    Testing no duplicate usernames...
    'no duplicate usernames'... PASSED ✓ 
    
    Testing user signin...
    'user signin'... PASSED ✓ 
    
    Testing no duplicate signins...
    'no duplicate signins'... PASSED ✓ 
    
    Testing user logout...
    'user logout'... PASSED ✓ 
    
    Testing password protection...
    'password protection'... PASSED ✓ 
    
    Testing another user sign in...
    'another user sign in'... PASSED ✓ 
    
    Testing 2fa command...
    '2fa command'... PASSED ✓ 
    
    Testing &2fa variable...
    '&2fa variable'... PASSED ✓ 
    
    Waiting for database to be written....
    -
    
    Testing testing 2fa...
    'testing 2fa'... PASSED ✓ 
    
    Testing testing for $creation immutability...
    'testing for $creation immutability'... PASSED ✓ 
    
    Testing testing for !channels immutability...
    'testing for !channels immutability'... PASSED ✓ 
    
    'User message sending'... PASSED ✓ 
    
    Finished without a hitch... your server implementation complies with the protocol!

