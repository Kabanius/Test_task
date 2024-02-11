# Welcome to GitHub Desktop!

This is your README. READMEs are where you can communicate what your project is and how to use it.

Write your name on line 6, save it, and then head back to GitHub Desktop.
def main(text):
    text = text.replace(" ", "")
    if len(text) == 5 and (int(text[:2]) and int(text[-2:])) <= 10:
        if "*" in text:
        elif "+" in text:
            decision = int(text[:2]) + int(text[-2:])
        elif "-" in text:
            decision = int(text[:2]) - int(text[-2:])
        elif "/" in text:
            decision = int(text[:2]) / int(text[-2:])
        return decision
    elif len(text) == 3:
        if "*" in text:
            decision = int(text[0]) * int(text[-1])
        elif "+" in text:
            decision = int(text[0]) + int(text[-1])
        elif "-" in text:
            decision = int(text[0]) - int(text[-1])
        elif "/" in text:
            decision = int(text[0]) / int(text[-1])
        return decision
    else:
        return "throws Exception"


print(main(input()))


