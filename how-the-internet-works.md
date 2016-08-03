# How does the Internet work?

> **This article discusses what the Internet is and how it works.**

The **Internet** is the backbone of the Web, the technical infrastructure that makes the Web possible. At its most basic, the Internet is a large network of computers which communicate all together.

When two computers need to communicate, you have to link them, either physically or wirelessly. Each computer on a network is connected to a special tiny computer called a _router_.

_Router_ makes sure that a message sent from a given computer arrives at the right destination computer. To send a message to computer B, computer A must send the message to the router, which in turn forwards the message to computer B and makes sure the message is not delivered to computer

By connecting computers to routers, then routers to routers, we are able to scale infinitely



The next step is to send the messages from our network to the network we want to reach. To do that, we will connect our network to an Internet Service Provider \(ISP\). An ISP is a company that manages some special _routers_ that link all together and can also access other ISPs' routers. So the message from our network is carried through the network of ISP networks to the destination network. The Internet consists of this whole infrastructure of networks.



### Finding computers

If you want to send a message to a computer, you have to specify which one. Thus any computer linked to a network has a unique address to identify it, called an "IP address" \(where IP stands for_Internet Protocol_\). It's an address made of a series of four numbers separated by dots, for example: `192.168.2.10`.

That's perfectly fine for computers, but we human beings have a hard time remembering that sort of address. To make things easier, we can alias an IP address with a human readable name called a _domain name_. For example, `google.com` is the domain name used on top of the IP address `173.194.121.32`. So using the domain name is the easiest way for us to reach a computer over the Internet.



### Internet and the web

As you might notice, when we browse the Web with a Web browser, we usually use the domain name to reach a website. Does that mean the Internet and the Web are the same thing? It's not that simple. As we saw, the Internet is a technical infrastructure which allows billions of computers to be connected all together. Among those computers, some computers \(called _Web servers_\) can send messages intelligible to web browsers. The _Internet_ is an infrastructure, whereas the _Web_ is a service built on top of the infrastructure. It is worth noting there are several other services built on top of the Internet, such as email and [IRC](https://developer.mozilla.org/en-US/docs/Glossary/IRC "IRC: IRC (Internet Relay Chat) is a worldwide chat system requiring an Internet connection and an IRC client, which sends and receives messages via the IRC server.").

