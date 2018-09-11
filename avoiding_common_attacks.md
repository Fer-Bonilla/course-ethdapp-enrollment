## Avoiding Common Attacks

The contract implementd is realy simple, and for this case atacks with patterns like Callstack Depth, Reentrancy and Private Information and Randomness
don't apply in this case

The only case for the basic function was the case of Integer overflow and underflow

### Integer overflow and underflow

```js
 function subscribe(
        bytes32 _code,
        string _fname,
        string _lname,
        string _id,
        uint8 _discount,
        string _email
    ) public payable {
        Course storage course = courses[_code];
        require(msg.value == 3 ether, "You didn't send 3 ether");
        course.students[msg.sender] = Student({
            id: _id,
            fname : _fname,
            lname : _lname,
            email : _email,
            session_codes : new bytes32[](0),
            isCertified : false
            });
    }
    }
```
