
The site is writing in ReStructuredText (rST) and built using Sphinx.  

If you are going to make changes to the site it would probably be best to setup a test environment for yourself. 

To do this:

1. Fork the repository on github.

2. Clone the fork to your workstation.

3. Setup a python virtual environment on your workstation. 

```
    virtualenv -p python3 venv
    . venv/bin/activate
```

4. Install sphinx in your virtual environment. 
```
    pip install sphinx
```

5. Make your changes.

6. Build the system with your changes. 
```
    make html
```

7. Point your web browser at the `_build/html` folder on your workstation
and make sure it all happened as expected. 

If it did and you are happy you can continue to deploy as follows: 

8. Commit your changes to your repository.

9. Push your repository back to github.

10. Send a pull request.

I'll receive the pull request, examine it, merge it, and push out the 
update.

