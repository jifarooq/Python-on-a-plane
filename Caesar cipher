import string

def cipherShift(crypt,n):

  # takes a message and does a cipherShift on it of n letters
  # If n is 3, 'a' changes to 'd', 'b' to 'e', etc, and 'cab' would become 'fde'
  
	message = ""
	key_lower = dict(zip(string.ascii_lowercase,string.ascii_lowercase[n:]+string.ascii_lowercase[:n]))
	key_upper = dict(zip(string.ascii_uppercase,string.ascii_uppercase[n:]+string.ascii_uppercase[:n]))
	key2 = dict(list(key_lower.items()) + list(key_upper.items()))
	
	for i in range(0,len(crypt)):
		message = message + key2.get(crypt[i],crypt[i])
	return message


# print all possible Ceasar ciphers
for a in range(0,25):
	print cipherShift(“spaghetti and meatballs”,a)
