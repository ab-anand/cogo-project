FROM ruby:2.2.2

WORKDIR /app
ADD Gemfile /app/Gemfile
ADD Gemfile.lock /app/Gemfile.lock
RUN bundle install --system

ADD . /app
RUN bundle install --system

EXPOSE 4567
CMD ["ruby", "hello_world.rb", "-o", "0.0.0.0"]
