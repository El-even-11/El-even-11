```python
class ReadMe:
    def __init__(self):
        self.name = 'Eleven'
        self.education = {
            'undergraduate': ['Shanghai Jiao Tong University', 'Computer Science']
        }
        self.contact = {
            'personal blog': ['https://El-even-11.github.io'],
            'email': ['zhao_ziqian@sjtu.edu.cn']
        }

    def knowing(self, what):

        if what is 'Who are you?':
            name = self.name
            education = self.education['undergraduate']
            return """
            I am {name}, an undergraduate in {university}, majoring in {major}.
            """.format(name=name,university=education[0], major=education[1])

        elif what is 'How to contact you?':
            blog = self.contact['personal blog']
            email = self.contact['email']
            return """
            Please contact me with email {email}, or my blog {blog}.
            """.format(email=email[0], blog=blog[0])

        else:
            return """
            ### Hi there 👋
            """

me = ReadMe()
```
