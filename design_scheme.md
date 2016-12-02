To DO
>
> a techincal sheet of a tipical smartID, with basic data first of all
> by smartID do we mean **etherReal-IÐ** from https://github.com/EtherReal-ID/documentation/blob/master/Roadmap%202016.md ? 
>
>
>


## smartID data structure. 


    open        =   Data is both unencrypted (in the clear) and searchable by anyone  (ie what you can find on google)
    hidden      =   Data is publicly known to exist but is inecsessable without decryption key  
    private     =   Data is verifiable but not searchable without authorisation
    constom     =   user can switch from public / hidden / private
    secret      =   Data is encrypted and   
    fixed       =   Noting can ever change this value.
    passive     =   ??

    (GEN)       =   Created during smartID generation
    (USR)       =   Can be updated/modified by user
							

### string public standard = 'etherRe.al 0.1';

    string public name;                 //  (GEN)       fixed  

    //birthday unix time
    uint public birthday;               //  (GEN)       fixed   open?

    //owner birth location
    string public bornlocation;         //  (GEN)       fixed   open?

    //State issued credentials  
        (e.g. passport, id card number)       
    string public state-issued-id;      //  (USR)       fixed   hidden  
    string public passport;             //  (USR)       fixed   hidden
    string public birth certificate     //  (USR)       fixed   hidden
    string public national insurance No.//  (USR)       fixed   hidden

    //the wallet controlling the smartid
    address public smartIDowner;        //  (MOD)       public  custom  

    address[] public wallets;           //  (MOD)       public  custom

    address[] public family;            //  (MOD)       public  custom

    //real address
    string public physicaladdress;	//  (MOD)       public  custom  (may change time after time)

    //email
        (can have many)    
    string public email;                //  (MOD)       public  custom


    address[] public validators;        //  (MOD)       public  passive
    uint[] public validatorsWhat;       //  (MOD)       public  passive

    address[] public validated;         //  (MOD)       public  passive
    uint[] public validatedWhat;        //  (MOD)       public  passive

    //last time image was updated
    uint public lastImageUpdate;        //  (   )       public  passive

    //last time a validation was made
    uint public lastCheck;		//  (   )       public  passive

    bool public checkemail;		//              public  passive
    bool public checkaddress;           //              public  passive
    bool public ispopa;                 //              public  passive
    bool public checkimage;             //              public  passive

    //how many times id was checked
    uint public idcheck;                //              public passive

    //how many times passport was checked
    uint public passportcheck;		//              public passive

    //how many times image was checked 
        (or each of the previous images!)
    uint public checkimageamount;       //              public passive

    //amount complaints
    uint public blackflags;		//   (GEN)      variable passive

    //points
    uint rating;			//              variable passive


    //wallet automatism
    mapping (address => uint256) public allowance;
    uint[] public allowances;
