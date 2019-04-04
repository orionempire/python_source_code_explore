c = compile('test.py', 'test.py', 'exec')#mistake
c = compile(open('test.py').read(), 'test.py', 'exec')
dir(c)
help(c)
c.co_code
type(c.co_code)
[byte for byte in c.co_code]
[ord(byte) for byte in c.co_code]
c = compile(open('Lecture_4.py').read(), 'Lecture_4.py', 'exec')
