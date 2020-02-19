# frozen_string_literal: true

require 'fileutils'
require 'asciidoctor'
require 'asciidoctor-revealjs'

BUILD_DIR = 'build'

task :convert do
  Asciidoctor.convert_file 'presentation.adoc',
                           backend: 'revealjs',
                           safe: Asciidoctor::SafeMode::UNSAFE,
                           to_dir: BUILD_DIR,
                           mkdirs: true
end

task default: :convert

task :clean do
  FileUtils.remove_entry_secure BUILD_DIR if File.exist? BUILD_DIR
end
