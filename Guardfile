notification :growl_notify

guard 'coffeescript', :output => '_site/js' do
  watch(/^.+\.coffee$/)
end

guard 'haml', :output => '_site' do
  watch(/^.+\.html.haml$/)
end

guard 'sass', output: '_site/css' do
  watch(/^.+\.scss$/)
end

guard 'shell' do
  watch(/img\/(\w*\.(jpg|png|gif|svg))/) {|m| `cp #{m[0]} _site/img/#{m[1]}` }
end

guard 'livereload' do
  watch(/^_site\/js\/.+\.js$/)
  watch(/^_site\/css\/.+\.css$/)
  watch(/^_site\/.+\.html$/)
end