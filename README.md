def main(text):
    text = text.replace(" ", "")
    b = "+*-/"
    decision = "throws Exception"
    for i in b:
        if text.find(i) > -1  and text.count(i) == 1 and int(text[:text.find(i)]) <= 10 and int(text[text.find(i) + 1:]) <= 10:
            if "+" in text:
                decision = int(text[:text.find("+")]) + int(text[text.find("+") + 1:])   
            elif "*" in text:
                ecision = int(text[:text.find("*")]) * int(text[text.find("*") + 1:])    
            elif "-" in text:
                decision = int(text[:text.find("-")]) - int(text[text.find("-") + 1:])     
            elif "/" in text:
                decision = int(text[:text.find("/")]) / int(text[text.find("/") + 1:])        
                decision = int(decision)
    else:
        return decision

print(main(input()))

