import re
mailtime = '^[a-z0-9]+[\._]?[a-z0-9]+[@]\w+[.]\w{2,3}$'  


def inputter():
	email = input("enter email ! \n")
	domain = re.split("@",email)[1]
	check(email,domain)


def isvalid(email):
	allowed_chars = set("+-_~.@" + "abcdefghijklmnopqrstuvwxyz" +
	                    "ABCDEFGHIJKLMNOPQRSTUVWXYZ" + "0123456789")
	return set(email).issubset(allowed_chars)
	



def check(email,domain):
	if (re.search(mailtime,email)):
		goodChars(email,domain)
	else:
		print("invalid email")
		inputter()


def goodChars(email,domain):
	if isvalid(email):
		real(domain)
	else:
		print("invalid chars")
		inputter()



def real(domain):
	with open("validmails.txt", 'r') as file:
		content = file.read()

		if domain in content:
			print("Email is valid")
		else:
			print("invalid domain")
			inputter()




inputter()
