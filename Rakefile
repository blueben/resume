task :default => 'convert:to_all'

namespace :convert do

  desc "Convert to text"
  task :to_txt do
    `textutil -convert txt BenjaminKruegerResume.rtf`
    puts "Converted to text"
 end

  desc "Convert to doc"
  task :to_doc do
    `textutil -convert doc BenjaminKruegerResume.rtf`
    puts "Converted to doc"
 end

  desc "Convert to PDF"
  task :to_pdf do
    `cupsfilter BenjaminKruegerResume.rtf > BenjaminKruegerResume.pdf`
    puts "Converted to PDF"
  end

  desc "Convert to all supported formats"
  task :to_all => [:to_txt, :to_doc, :to_pdf] do
    puts "Done"
  end

end
