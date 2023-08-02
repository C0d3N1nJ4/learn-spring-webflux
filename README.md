# learn-spring-webflux

A simple reactive web application with Spring Webflux to learn the basic concepts and configurations of this framework.

Notes:
- The lowest component of Spring Webflux is the org.springframework.http.server.reactive.HttpHandler, which is a reactive HTTP request handler.












## Spring Webflux Architecture
- The HttpHandler is wrapped by the org.springframework.web.server.adapter.WebHttpHandlerBuilder, which is a builder for the HttpHandler.
- The WebHttpHandlerBuilder is wrapped by the org.springframework.http.server.reactive.ReactorHttpHandlerAdapter, which is a HttpHandler that adapts to Reactor Netty.
- The ReactorHttpHandlerAdapter is wrapped by the org.springframework.boot.web.embedded.netty.NettyWebServer, which is a Netty web server.
- The NettyWebServer is wrapped by the org.springframework.boot.web.embedded.netty.NettyWebServerFactory, which is a factory for the NettyWebServer.
- The NettyWebServerFactory is wrapped by the org.springframework.boot.web.reactive.server.ReactiveWebServerFactory, which is a factory for the NettyWebServer.
- The ReactiveWebServerFactory is wrapped by the org.springframework.boot.web.reactive.server.ReactiveWebServerFactoryAutoConfiguration, which is a configuration for the ReactiveWebServerFactory.
- The ReactiveWebServerFactoryAutoConfiguration is wrapped by the org.springframework.boot.autoconfigure.web.reactive.ReactiveWebServerFactoryAutoConfiguration, which is a configuration for the ReactiveWebServerFactory.
- The ReactiveWebServerFactoryAutoConfiguration is wrapped by the org.springframework.boot.autoconfigure.web.reactive.ReactiveWebServerFactoryConfiguration.EmbeddedReactiveWebServerFactoryCustomizerConfiguration, which is a configuration for the ReactiveWebServerFactory.
