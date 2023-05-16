def userInput():
	userPassword = input("enter your password: ")
	passwordInteg(userPassword)


def is_valid_password(userPassword):
	allowed_chars = set("!%&*+=" + "abcdefghijklmnopqrstuvwxyz" +
	                    "ABCDEFGHIJKLMNOPQRSTUVWXYZ" + "0123456789")
	return set(userPassword).issubset(allowed_chars)


def passwordInteg(userPassword):
	if len(userPassword) < 8:
		print("too short")
		userInput()

	elif len(userPassword) > 15:
		print("too long")
		userInput()

	else:
		print("forbidden characters")
		userInput()

