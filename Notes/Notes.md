notes = []

loop do
  puts "\n1. Add Note\n2. View Notes\n3. Exit"
  choice = gets.chomp.to_i

  case choice
  when 1
    print "Enter note: "
    notes << gets.chomp
  when 2
    puts "Notes:"
    notes.each_with_index { |note, i| puts "#{i + 1}. #{note}" }
  when 3
    break
  else
    puts "Invalid choice"
  end
end
