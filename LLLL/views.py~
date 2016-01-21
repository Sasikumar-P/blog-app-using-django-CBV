from django.http import HttpResponse
from django.views.generic import TemplateView,ListView
from django.views.generic.edit import CreateView, UpdateView, DeleteView
from django.core.urlresolvers import reverse_lazy

from LLLL.models import Post

class BookList(ListView):
    model = Post

class BookCreate(CreateView):
    model = Post
    fields = ['author', 'body','title']
    success_url = reverse_lazy('books_cbv:book_list')

class BookUpdate(UpdateView):
    model = Post
    fields = ['author', 'body','title']
    success_url = reverse_lazy('books_cbv:book_list')

class BookDelete(DeleteView):
    model = Post
    success_url = reverse_lazy('books_cbv:book_list')

# Create your views here.
