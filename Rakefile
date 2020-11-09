# frozen_string_literal: true

require 'rubygems'
require 'bundler/setup'
require 'dotenv/load'
require 'dotenv/tasks'
require 'twitchbot'

desc 'Start the bot'
task start_bot: :dotenv do
  bot = Twitchbot::Bot.new do |bot|
    bot.username = ENV['BOT_USERNAME']
    bot.password = ENV['BOT_PASSWORD']
    bot.channel = ENV['BOT_CHANNEL']
    bot.plugins = []
    bot.debug = true
  end

  bot.start
end
