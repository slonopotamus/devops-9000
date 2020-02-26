# frozen_string_literal: true

require 'asciidoctor-diagram'
require 'asciidoctor-revealjs'
require 'rake/clean'

task :default do
  FileUtils.cp_r 'images', 'build'
  Asciidoctor.convert_file 'presentation.adoc',
                           backend: 'revealjs',
                           safe: Asciidoctor::SafeMode::UNSAFE,
                           to_dir: 'build'
end

CLEAN.include 'build'
