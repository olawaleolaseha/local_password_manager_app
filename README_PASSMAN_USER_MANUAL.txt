PassMan is a "local" password manager application. It is different from other password managers like Keepass, Lastpass etc. because this can be useful in a situation where internet is 
not allowed in your local network (and therefore you cannot use the popular internet based password manager apps to manage passwords on the systems on your local network).
The motivation to create this password manager is from my experience with Operational Technology (OT) or Industrial Automation and Control Systems (IACS) where industry best standards, risks mitigation measures and compliance requirements requires that internet connection be prohibited in Purdue Layer 0/1/2 systems. In situations like this, and other
similar ones, you could use PassMan to manage the passwords of systems locally. 

To start, go to PassMan > dist and double-click on "passman_vlt_mod_main.exe"


On first use, a database of the passwords stored in the vault is created.
The passwords are not stored in the database in clear text. Instead the hashed values (using sha256) are stored.

You can locate the hashed password database in path PassMan/dist...

If you lose or forget the master password, you will need to reset it. The best way to reset it is to delete the passman.db file from the Path PassMan/dist. Note that you will lose all the passwords previously stored in this vault. This is a security feature to protect passwords stored in the fault. So, make sure you do not forget the master password.

Also, only use this application to manage/store passwords that you can reset from the platform or account that they are being used. That way, if you have to reset tha master password, you could go back to your platform or applications to use the 'forgot password?' or 'reset password' function on them, and can then come and store the new passwords on PassMan. It is advisable that you use the Password Generator function in PassMan to generate your passwords for your varoius applications.

Again, IF 'FORGOT PASSWORD' OR 'RESET PASSWORD' FUNCTION IS NOT AVAILABLE ON THE APPLICATION YOU ARE USING PASSMAN TO MANAGE ITS PASSWORD, PLEASE DO NOT USE PASSMAN. IF YOU DO, YOU STAND A RISK OF BEING PERMANENTLY LOCKED OUT OF YOUR APPLICATION IF YOU FORGET YOUR PASSMAN MASTER PASSWORD!