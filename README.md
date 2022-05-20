# ooc-project-IT21391668
ooc-project-IT21391668 created by GitHub Classroom
//IT21391668

//Class for Registered User
Class registeredUser {

protected:
string username ;
string password ;
string email ; 
string firstName ; 
string lastName ; 
int phone ;

public:
registeredUser(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone );
void searchProperty();
~registeredUser() ;

};

//constructor
registeredUser :: registeredUser(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone ) {

username = m_username ;
password = m_password ;
email = m_email ;
firstName = m_fistName ;
lastName = m_lastName ;
phone = m_phone ;
}

//destructor
registeredUser :: ~registeredUser(){
cout << "Deleting registeredUser" << endl ;
}

//Class for Buyer
Class Buyer: public registeredUser {

protected:
string username ;
string password ;
string email ; 
string firstName ; 
string lastName ; 
int phone ;
int appointmentNumber ;

public:
Buyer(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone );
void searchProperty();
void requestAppointment() ;
~Buyer() ;

};

//constructor
Buyer :: Buyer(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone ) {

username = m_username ;
password = m_password ;
email = m_email ;
firstName = m_fistName ;
lastName = m_lastName ;
phone = m_phone ;
}

//destructor
Buyer :: ~Buyer(){
cout << "Deleting Buyer" << endl ;
}

//Class for Seller
Class Seller: public registeredUser{

protected:
string username ;
string password ;
string email ; 
string firstName ; 
string lastName ; 
int phone ;
int appointmentNumber ;
int advertisementID ;
int requestNumber ;
string paymentID ;

public:
Seller(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone );
void requestAppointment();
void postAdvertisement() ;
void requestVerification() ;
void makePayment() ;
void getAdvertisementList(Profile *PRO) ;
~Seller() ;

};

//constructor
Seller :: Seller(string m_username , string m_password , string m_email , string m_fistName . string m_lastName , int m_phone ) {

username = m_username ;
password = m_password ;
email = m_email ;
firstName = m_fistName ;
lastName = m_lastName ;
phone = m_phone ;
}

//destructor
Seller :: ~Seller(){
cout << "Deleting Seller" << endl ;
}
