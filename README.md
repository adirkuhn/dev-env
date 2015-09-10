# dev-env
Development Environment

Setup for web development with PHP, Ruby and Python.

# Mac
## Mac 10.8.*
### Command Line Tools

Install Command Line Tools for your mac version (https://developer.apple.com/downloads/)

### Install Git

For version control, download from (https://git-scm.com/download/mac)

### Ruby

#### Remove default installed ruby
Delete ruby references from /usr/bin

```
$ sudo rm /usr/bin/ruby
$ sudo rm /usr/bin/rails
$ sudo rm /usr/bin/gem
```

#### Install rbenv and ruby-build

Clone the project rbenv

```
$ git clone https://github.com/sstephenson/rbenv.git ~/.rbenv
```

Add binaries to system PATH `.bashrc` or `.zshrc`

```
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
```

Clone ruby-build

```
$ git clone https://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
```

And finally install ruby

```
$ rbenv install 2.2.3
$ rbenv global 2.2.3
$ gem install rake
$ gem intall bundle
```
