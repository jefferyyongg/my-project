Name three components of your solution:

I think the three most important components of this last assignments were, figuring out how to create ssh keys and connecting them to your github repo. Also learning how to configure your vps the right way (giving permissions to certain folders etc.), and lastly github actions logging into your vps.

Discuss three problems that you encountered along the way and how you solved them:

1. Github actions succeeded but code not showing up in vps
   after pulling code to the vps i still had to make sure i restart the vps so that my new code in implemented properly.

2. Running pytest before running deployment script
   a bit of googling and found that i could chain jobs by using the "needs:" command, so that my deployment code needs run-test to succeed before it can run.

3. Github actions giving me authentication errors
   after pushing my new code, github actions ran it and after succeeding the pytest it wouldnt connect to the vps and return unable to autenticate. I fixed this by using edcsa insead of rsa and gave the authorized_keys file permissions with the "chmod" command.
