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


