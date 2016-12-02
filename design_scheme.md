

To DO
>
> a techincal sheet of a tipical smartID, with basic data first of all
>
>
>
>


## smartID data structure. 

 

    (GEN) = created during smartID generation
							
    string public standard = 'EtherRe.al 0.1';

    string public name;			//(GEN) fixed  

    //birthday unix time
    uint public birthday;		//(GEN) fixed public?

    //owner birth location
    string public bornlocation;		//(GEN) fixed public

    //real id card number       
    string public id;			//(GEN) fixed hidden

    //real passport number   
    string public passport;		//fixed	hidden

    //the wallet controlling the smartid
    address public smartIDowner;        //public custom  

    address[] public wallets;		//public custom

    address[] public family;		//public custom

    //real address
    string public physicaladdress;	//public custom (may change time after time)

    //email
    string public email;		//public custom


    address[] public validators;	//public passive
    uint[] public validatorsWhat;	//public passive

    address[] public validated;		//public passive
    uint[] public validatedWhat;	//public passive

    //last time image was updated
    uint public lastImageUpdate;  	//public passive

    //last time a validation was made
    uint public lastCheck;		//public passive

    bool public checkemail;		//public passive
    bool public checkaddress;		//public passive
    bool public ispopa;			//public passive
    bool public checkimage;		//public passive

    //how many times id was checked
    uint public idcheck;		//public passive

    //how many times passport was checked
    uint public passportcheck;		//public passive

    //how many times image was checked (or each of the previous images!)
    uint public checkimageamount;	//public passive

    //amount complaints
    uint public blackflags;		//variable passive

    //points
    uint rating;			//variable passive


    //wallet automatism
    mapping (address => uint256) public allowance;
    uint[] public allowances;




















