```python
from bookshelf.models import Book

book = Book.objects.create(
    title="1984",
    author="George Orwell",
    publication_year=1949
)

book


book = Book.objects.get(title="1984")
book.title, book.author, book.publication_year


book = Book.objects.get(title="1984")
book.title, book.author, book.publication_year



book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()

book.title


book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

Book.objects.all()

