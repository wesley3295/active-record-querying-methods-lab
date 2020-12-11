class CreateShows < ActiveRecord::Migration[5.2]
   def change
    create_table :shows do |t|
        t.string :name
        t.string :day
        t.string :newtwork
        t.integer :rating
        end
    end
end

class AddSeasonToShows < ActiveRecord::Migration[5.2]
   def change
        add_column :shows, :season, :string
   end
end