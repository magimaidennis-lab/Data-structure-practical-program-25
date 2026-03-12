# Data-structure-practical-program-25
def check(s):
    stack = []
    for i in s:
        if i == '(':
            stack.append(i)
        elif i == ')':
            if not stack:
                return "Not Balanced"
            stack.pop()
    if not stack:
        return "Balanced"
    else:
        return "Not Balanced"

exp = "(())()"
print(check(exp))
Balanced
